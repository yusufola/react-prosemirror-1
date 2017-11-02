An editor for content stored as ProseMirror JSON.

```js
const options = require('@aeaton/react-prosemirror-config-default')

initialState = {
  doc: {}
};

<div>
    <h2>Input</h2>
    
    <Editor 
      options={options}
      onChange={doc => setState({ doc })}
    />
    
    <h2>Output</h2>
    
    <pre><code>{JSON.stringify(state.doc, null, 2)}</code></pre>
</div>
```