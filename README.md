# Pagination React Hooks
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/berat/pagination-react-hooks/issues) [![npm version](https://badge.fury.io/js/pagination-react-hooks.svg)](https://badge.fury.io/js/pagination-react-hooks)
[![https://nodei.co/npm/pagination-react-hooks.png?downloads=true&downloadRank=true&stars=true](https://nodei.co/npm/pagination-react-hooks.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pagination-react-hooks)

> #### Pagination component prepared with React hooks. Load and use.
> My first component as an open source after learning React. If you want to contribute, I am waiting for you in the issue section.

<br>

## Installation
Install `pagination-react-hooks` with npm:

`npm i pagination-react-hooks`

with yarn:

`yarn add pagination-react-hooks`

<br>

## Example

To be practical you can see live in my react application [https://practical-react.herokuapp.com](https://practical-react.herokuapp.com).


<br>

## Usage
Add the component to the section you want to show and remember to use the parameters. That's all.

```js
import React from 'react';
import Pagination from './Pagination';

const Content = () => {
    const show = (value) => (
        <li className="card">
            <span>{value.name}</span>         
        </li>
    )
    return (
        <Pagination
            posts={posts}
            Show={show}
            displayNumber="7"
            previousText="Önceki"
            nextText="Sonraki"
        />
    )
}
export default Content;
```

<br>


## Params

| Parameters        | Description                        
|------------------|------------------------------------|
| posts         | The array of content to display.                 |
| Show         | The theme you want to sho your content                 |
| displayNumber         | The maximum number of content to display on the page.                |
| previousText         | Previous button text                 |
| nextText         | Next button text                |