<template>
  <div style="margin: 20px;">
        <el-upload
          ref="videoUpload"
          :file-list="videoList"
          action="http://localhost:8080/pdl-index/uploadVideo_UploadAction.pdl!"
          :on-change="onVideoChange"
          accept="video/*"
        >
          <el-button size="small" type="primary">点击上传</el-button>
          <span style="color:#909399;font-size:14px;    margin-left: 8px;">请上传mp4文件</span>
        </el-upload>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        videoList:[],
        input: 'Hello Element UI!'
      };
    },
    methods:{
      onVideoChange(file,fileList){
      }
    }
  };
</script>
