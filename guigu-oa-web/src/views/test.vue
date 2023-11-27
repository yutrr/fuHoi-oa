<template>
  <div>
    <div>账号切换</div>
    <button @click="zs()" type="default" size="mini">张三</button>
    <button @click="lisi()" type="default" size="mini">李四</button>
    <button @click="zzjl()" type="default" size="mini">张总经理</button>
    <button @click="admin()" type="default" size="mini">admin</button>
    <div>当前token：{{ token }}</div>
  </div>
</template>

<script>
export default {
  name: "Test",

  data() {
    return {
      token: ''
    };
  },

  created(){
    this.token = window.localStorage.getItem('token')
  },

  methods: {
    admin() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNLOwNDE2MTY00VEqLU4t8kwBikGYeYm5qUAtiSm5mXlKtQB3na82QgAAAA.tXmOwlstiWG9BmakrLn9peIya92k20iURObVaI-i7rJvhOnfxJWbi7mFWiER3b7JKPLsCZ3nWAK50EWjn5RmcQ'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    zs() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNLOwNDE2MTE01lEqLU4t8kxRsjKHMPMSc1OBWqoyEvPSixPzlGoBPuux80UAAAA.9anPOXDtPEFmyIj-2wSpGngh3K2r04RI_g7l-D0Re6lXfUYikImnUZ7_6hk7Yz7Pio9XDtoy52Y2PT6TfmKLaw'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    zzjl() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDM3NjMwNLYw11EqLU4t8kxRsjKFMPMSc1OBWqqqsnKUagGHebUNQQAAAA.FcCkD6QfaP8bd_3MYsRD6Tp9wr9JSRFWIUuIdG5O7XxhIeyWfzGLp40_Lesx_kWMMaaskh_ba3NrTlj8-nP6OA'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    lisi() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNLOwNDE2MbGw0FEqLU4t8kxRsjKBMPMSc1OBWnIyizOVagGqvFQFQQAAAA.0fQsvA5p7149vF9ZKhhZTJlyh_yQxXeSeB4Pr27S3nDpvdaQKoP4V4lx7GsgFO7V81Fvs76rI6h0rLJ8vVxnFA'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    }
  }
}
</script>
