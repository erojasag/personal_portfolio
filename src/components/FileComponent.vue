<template>
  <div id="app">
    <h2>Download My CV</h2>
    <button @click="downloadFile()">Download</button>
  </div>
</template>

<script>
import axios from "axios";
export default {
  mounted() {
    this.downloadFile();
  },
  methods: {
    async downloadFile() {
      axios({
        url: "https://drive.google.com/file/d/1uPyeUOaxJOHSV1uwmKvBV1uiCeuvw2iF/view?usp=share_link",
        method: "GET",
        responseType: "blob",
        headers: {
          "Content-Type": "application/pdf",
          "Access-Control-Allow-Origin": "*",
        },
      }).then((res) => {
        let FILE = window.URL.createObjectURL(new Blob([res.data]));

        let docUrl = document.createElement("x");

        docUrl.href = FILE;
        docUrl.setAttribute("download", "my-cv.pdf");
        document.body.appendChild(docUrl);
        docUrl.click();
      });
    },
  },
};
</script>

<style>
</style>