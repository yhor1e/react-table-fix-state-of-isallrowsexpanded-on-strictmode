This repository is applying [react-table #3471](https://github.com/tannerlinsley/react-table/pull/3471) to [expanding example](https://github.com/tannerlinsley/react-table/tree/8c77b4ad97353a0b1f0746be5b919868862a9dcc/examples/expanding).

`yarn` and `yarn start` to run this example and check it.

I changed the below.

`src/App.js`

```diff
    <Styles>
+      <React.StrictMode>
        <Table columns={columns} data={data} />
+      </React.StrictMode>
    </Styles>
```

`package.json`

```diff
 "dependencies": {
   "namor": "^1.1.2",
   "react": "^16.8.6",
   "react-dom": "^16.8.6",
   "react-scripts": "3.0.1",
-   "react-table": "latest",
+   "react-table": "https://github.com/yhor1e/react-table#fix-state-of-isallrowsexpanded-on-strictmode",
   "styled-components": "^4.3.2"
 },
```

---

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app) and Rescripts.

You can:

- [Open this example in a new CodeSandbox](https://codesandbox.io/s/github/tannerlinsley/react-table/tree/master/examples/expanding)
- `yarn` and `yarn start` to run and edit the example
