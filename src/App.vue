<template>
  <div>
    <Header :appTitle="title" />
    <WebMap />
  </div>
</template>

<script>

import Header from './components/Header';
import WebMap from './components/WebMap';

import { title } from './config';

export default {
    name: 'App',
    components: { Header, WebMap },
    data: () => (
      {
        title
      }
    )
};

</script>

<style scoped>
    div  {
      display: flex;
      flex-direction: column;
      padding: 0;
      margin: 0;
      width: 100%;
      height: 100%;
    }
</style>