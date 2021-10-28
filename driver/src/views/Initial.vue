<template>
  <div class="container">
    <div class="front">
      <b-card bg-variant="success" text-variant="white" header="Instructions" align="left">
        <p>Charles Jiang 14848</p>
        <p>Please choose one application to run</p>
      </b-card>
    </div>

    <div class="front">
        <el-button
            type="success"
            @click="jupyterNotebook"
            round
            style="margin-top: 10px; margin-bottom: 10px"
        >
            Jupyter-Notebook
        </el-button>
        <el-button
            type="success"
            @click="spark"
            round
            style="margin-top: 10px; margin-bottom: 10px"
        >
            Spark
        </el-button>
        <el-button
            type="success"
            @click="hadoop"
            round
            style="margin-top: 10px; margin-bottom: 10px"
        >
            Hadoop
        </el-button>
        <el-button
            type="success"
            @click="sonar"
            round
            style="margin-top: 10px; margin-bottom: 10px"
        >
            Sonar
        </el-button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'initial',
  data () {
    return {
      userAgent: null
    }
  },

  methods: {
    jupyterNotebook () {
      window.location.href = 'http://my-jupyter-notebook:81'
    },
    spark () {
      var currentHost = window.location.host
      window.location.href = 'http://' + currentHost + '/spark:8080'
    },
    hadoop () {
      var currentHost = window.location.host
      window.location.href = 'http://' + currentHost + '/hadoop:50070'
    },
    sonar () {
      var currentHost = window.location.host
      window.location.href = 'http://' + currentHost + '/sonar:9000'
    }
  }
}
</script>
