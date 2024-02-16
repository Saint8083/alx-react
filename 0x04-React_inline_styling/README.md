# 0x04. React inline styling


DOM Elements
These docs are old and won’t be updated. Go to react.dev for the new React docs.

These new documentation pages teach modern React and include live examples:

Common components (e.g. <div>)
<input>
<option>
<progress>
<select>
<textarea>
React implements a browser-independent DOM system for performance and cross-browser compatibility. We took the opportunity to clean up a few rough edges in browser DOM implementations.

In React, all DOM properties and attributes (including event handlers) should be camelCased. For example, the HTML attribute tabindex corresponds to the attribute tabIndex in React. The exception is aria-* and data-* attributes, which should be lowercased. For example, you can keep aria-label as aria-label.

Differences In Attributes
There are a number of attributes that work differently between React and HTML:

checked
The checked attribute is supported by <input> components of type checkbox or radio. You can use it to set whether the component is checked. This is useful for building controlled components. defaultChecked is the uncontrolled equivalent, which sets whether the component is checked when it is first mounted.

className
To specify a CSS class, use the className attribute. This applies to all regular DOM and SVG elements like <div>, <a>, and others.

If you use React with Web Components (which is uncommon), use the class attribute instead.

dangerouslySetInnerHTML
dangerouslySetInnerHTML is React’s replacement for using innerHTML in the browser DOM. In general, setting HTML from code is risky because it’s easy to inadvertently expose your users to a cross-site scripting (XSS) attack. So, you can set HTML directly from React, but you have to type out dangerouslySetInnerHTML and pass an object with a __html key, to remind yourself that it’s dangerous. For example:

function createMarkup() {
  return {__html: 'First &middot; Second'};
}

function MyComponent() {
  return <div dangerouslySetInnerHTML={createMarkup()} />;
}
