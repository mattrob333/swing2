<script>
       document.getElementById('videoInput').addEventListener('change', function(event) {
        const file = event.target.files[0];
        const url = URL.createObjectURL(file);
        const videoPlayer = document.getElementById('videoPlayer');
        videoPlayer.src = url;
        videoPlayer.load();
        videoPlayer.play();
    }); // Swing Compare page logic
</script>

<h1>Swing Compare</h1>
<div id="video-upload-container">
    <input type="file" accept="video/*" id="videoInput" />
    <video id="videoPlayer" controls width="250">
        <track kind="captions" src="path_to_your_captions_file.vtt" srclang="en" label="English">
        Your browser does not support the video tag.
    </video>
</div>
<p>hey</p>