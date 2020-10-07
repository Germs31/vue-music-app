<template>
  <div id="app">
    <header>
      <h1>My Music</h1>
    </header>
    <main>
      <section class="player">
        <h2 class="song-title">{{ current.title}}</h2>
        <span>{{current.artist}}</span>
      </section>
    </main>
  </div>
</template>

<script>

export default {
  name: 'App',
  // data is state
  data () {
    return {
      current: {},
      songs: [
      {
        title: 'Etta',
        artist: 'German',
        src: require('./assets/etta.mp3')
      },
      {
        title: 'Rhine',
        artist: 'German',
        src: require('./assets/rhine.mp3')
      }
      ]
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

header {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 15px;
  background: #212121;
  color: #fff;
}
</style>
