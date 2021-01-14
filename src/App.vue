<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
// import osc from 'osc'

// // Create an osc.js UDP Port listening on port 57121.
// var udpPort = new osc.UDPPort({
//   localAddress: '0.0.0.0',
//   localPort: 57121,
//   metadata: true
// })

// // Listen for incoming OSC messages.
// udpPort.on('message', function (oscMsg, timeTag, info) {
//   console.log('An OSC message just arrived!', oscMsg)
//   console.log('Remote info is: ', info)
// })

// // Open the socket.
// udpPort.open()

// // When the port is read, send an OSC message to, say, SuperCollider
// udpPort.on('ready', function () {
//   udpPort.send({
//     address: '/s_new',
//     args: [
//       {
//         type: 's',
//         value: 'default'
//       },
//       {
//         type: 'i',
//         value: 100
//       }
//     ]
//   }, '127.0.0.1', 57110)
// })

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
