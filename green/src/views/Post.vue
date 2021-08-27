<template>
  <div class="mt-3">
    <div class="post-card">
      <div class="card">
        <div class="card-header">
          投稿画面
        </div>
        <div class="card-body">
          <form class="upload-images p-0 border-0" id="new_post" enctype="multipart/form-data" action="">
            <div class="form-group">
              <div class="col-auto pr-0">
                <img class="post-profile-icon round-img" src="../assets/logo.png"/>
              </div>
              <div class="col pl-0">
                <input class="form-control border-0" placeholder="キャプションを書く" type="text" name="caption"
                  value="" />
              </div>
            </div>
            <div class="mb-3">
              <input type="file" name="photo" accept="image/jpeg,image/gif,image/png" />
            </div>
            <button type="submit" name="commit" class="btn btn-primary" >投稿する</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.mt-3{
  background-color: rgb(216, 202, 202);
  width:100%;
  height: 100vh;
  
}
.post-card{
  background-color: white;
  width:80%;
  margin: 0 auto;
  padding-bottom: 20px;
  border-radius: 5px;
}
.card-header{
  padding:20px;
  font-size: 20px;
  background-color: #eeeeee;
  border-top-right-radius: 5px;
  border-top-left-radius: 5px;
}
.card-body{
  margin: 30px;
}
.post-profile-icon{
  width:80px;
  height:80px;
  border-radius: 50%;
  margin-right: 10px;
}
.form-group{
  display: flex;
}
.form-control {
  border: 1px solid #ffffff;
  font-size: inherit;
  padding-bottom:70px;
}

input {
  margin: 10px 0;
  padding:10px 150px 10px 5px;
}

button{
  padding:10px 50px ;
  font-size: 16px;
  color: #fff;
  background-color: #007bff;
  border-color: #007bff;
}

.devise-link {
  text-align: center;
  margin: 16px 0;
}

#wrapper {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

footer {
  margin-top: auto;
}

.card-wrap {
  margin: 40px 0px;
}

.no-text-decoration:hover {
  text-decoration: none;
}

.black-color {
  color: #262626;
}

.parts {
  margin: 12px 0;
}

.post-time {
  margin:0;
  color:#999;
  font-size:10px;
}

.post-sub-text {
  text-decoration: none;
  color: #262626;
}
</style>