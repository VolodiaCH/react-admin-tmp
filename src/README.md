Steps that I've made:

npx create-react-app my-app

cd my-app

npm start

npm i -s react-admin ra-data-json-server prop-types

Then successfully went through https://marmelab.com/react-admin/Tutorial.html until section "Mapping API Endpoints With Resources".

I've got an reported error after I performed:

import React from 'react';

import { Admin, Resource, ListGuesser } from 'react-admin';

import jsonServerProvider from 'ra-data-json-server';

const dataProvider = jsonServerProvider('http://jsonplaceholder.typicode.com');

const App = () => (

<Admin dataProvider={dataProvider}>

<Resource name="users" list={ListGuesser} />

</Admin>

);

export default App;
