# Yt-downloader-

<div class="col-md-6 offset-md-3 mt-5">
    <div class="card">
      <div class="card-header bg-info">
        <center><h5><p><span style="color: White; font-family: verdana; font-size: x-large;"><b>&nbsp; YouTube Video Downloader</b></span></p>
      </div>
      <div class="card-body">
        <div class="row">
          <div class="col-md-12">
            <div class="form-group">
              <label class="text-weight"><b>Enter Yt Video Link:</b></label>
              <input type="txt" name="link" class="form-control link" required>
            </div>
          </div>
        </div>
        <form class="form-download">
          <div class="row">
            <div class="col-md-12">
              <div class="form-group">
                <label class="text-weight"><b>Select Video Format:</b></label>
                <select class="form-control formte" required>
                  <option selected disabled>Select Video Format</option>
                  <option value="mp3">Mp3</option>
                  <option value="mp4a">144 Mp4</option>
                  <option value="360">360 Mp4</option>
                  <option value="480">480 Mp4</option>
                  <option value="720">720 Mp4</option>
                  <option value="1080">1080 Mp4</option>
                  <option value="4k">4k Mp4</option>
                  <option value="8k">8k Mp4</option>
                </select>
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col-md-12">
              <div class="form-group mt-4 download-video">
                <button class="btn btn-success btn-block click-btn-down" type="submit">Click Here</button>
              </div>
            </div>
          </div>
        </form>
      </div>
    </div>
  </div>

::CSS::

<style>
  * {
margin: 0;
padding: 0;
}

.mt-5, .my-5 {
    margin-top: 0rem!important;
}

#hd {    
  width:100%;    
  height:390px;      
  margin:0 0 50px 0;    
  }  


.custom-shape-divider-bottom-1610026357 {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}

.custom-shape-divider-bottom-1610026357 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 183px;
}

.custom-shape-divider-bottom-1610026357 .shape-fill {
    fill: #FFFFFF;
}
  
  </style>


::JS::

<script type="text/javascript">
  $(".click-btn-down").click(function(){
      var link = $(".link").val();
    var fromate = $(".formte").children("option:selected").val();
    var src =""+link+"="+fromate+"";
    downloadVideo(link,fromate);
  });
  function downloadVideo(link,fromate) {
      $('.download-video').html('<iframe style="width:100%;height:60px;border:0;overflow:hidden;" scrolling="no" src="https://loader.to/api/button/?url='+link+'&f='+fromate+'"></iframe>');
  }
</script>


