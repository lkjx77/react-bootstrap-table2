---
id: getting-started
title: Getting Started
sidebar_label: Getting Started
---

## Installation

> Due to `react-bootstrap-table2` already taked on npm so that our npm module name is **`react-bootstrap-table-next`**. Anyway, we still use or mention `react-bootstrap-table2` in any our git repository, offical website and documents!!, ony the npm name is different!!!!

```sh
$ npm install react-bootstrap-table-next --save
```

## Add CSS

> `react-bootstrap-table2` need you to add bootstrap css in your application firstly. About bootstrap css, we only compatible with bootstrap 3 but will start to compatible for bootstrap 4 on **v0.2.0**

Finish above step, let's add the `react-bootstrap-table2` styles: 

```js
// es5 
require('react-bootstrap-table-next/dist/react-bootstrap-table2.min.css');

// es6
import 'react-bootstrap-table-next/dist/react-bootstrap-table2.min.css';
```

## Your First Table

```js
import BootstrapTable from 'react-bootstrap-table-next';

const products = [ ... ];
const columns = [{
  dataField: 'id',
  text: 'Product ID'
}, {
  dataField: 'name',
  text: 'Product Name'
}, {
  dataField: 'price',
  text: 'Product Price'
}];

export default () =>
  <BootstrapTable keyField='id' data={ products } columns={ columns } />
```