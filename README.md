<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الذباب الإلكتروني</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            direction: rtl;
            text-align: right;
            padding: 20px;
        }

        h1 {
            text-align: center;
            color: #333;
        }

        .video-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            justify-content: center;
        }

        .video-item {
            background-color: #fff;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        /* جعل أبعاد الفيديو متجاوبة */
        .video-item iframe {
            display: block;
            margin-bottom: 10px;
            width: 100%;
            height: auto;
            aspect-ratio: 16 / 9; /* تحافظ على نسبة العرض إلى الارتفاع (16:9) */
        }

        .controls {
            text-align: center;
        }

        .controls button, .controls input {
            padding: 8px 15px;
            margin-top: 5px;
            border-radius: 5px;
            border: 1px solid #ccc;
            font-size: 14px;
        }
            
        .controls button {
            background-color: #007bff;
            color: white;
            border: none;
            cursor: pointer;
        }

        .controls button:hover {
            background-color: #0056b3;
        }

        .controls .copy-button {
            background-color: #28a745;
        }

        .controls .copy-button:hover {
            background-color: #218838;
        }

        .controls input {
            width: 80%;
            padding: 8px;
            margin-bottom: 10px;
            box-sizing: border-box;
            text-align: left;
            direction: ltr;
        }

        /* قواعد CSS الخاصة بالهواتف */
        @media (max-width: 768px) {
            .video-container {
                grid-template-columns: 1fr; /* عرض فيديو واحد لكل سطر */
            }
        }
    </style>
</head>
<body>

    <h1>الذباب الإلكتروني</h1>

    <div class="video-container">
        <div class="video-item">
            <input type="text" id="videoUrl1" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video1', 'videoUrl1')">تشغيل</button>
            <iframe id="video1" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video1')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl1')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video1', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>

        <div class="video-item">
            <input type="text" id="videoUrl2" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video2', 'videoUrl2')">تشغيل</button>
            <iframe id="video2" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video2')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl2')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video2', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>

        <div class="video-item">
            <input type="text" id="videoUrl3" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video3', 'videoUrl3')">تشغيل</button>
            <iframe id="video3" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video3')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl3')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video3', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>

        <div class="video-item">
            <input type="text" id="videoUrl4" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video4', 'videoUrl4')">تشغيل</button>
            <iframe id="video4" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video4')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl4')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video4', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>

        <div class="video-item">
            <input type="text" id="videoUrl5" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video5', 'videoUrl5')">تشغيل</button>
            <iframe id="video5" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video5')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl5')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video5', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>

        <div class="video-item">
            <input type="text" id="videoUrl6" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video6', 'videoUrl6')">تشغيل</button>
            <iframe id="video6" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video6')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl6')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video6', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>
            
        <div class="video-item">
            <input type="text" id="videoUrl7" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video7', 'videoUrl7')">تشغيل</button>
            <iframe id="video7" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video7')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl7')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video7', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>

        <div class="video-item">
            <input type="text" id="videoUrl8" placeholder="الصق رابط يوتيوب هنا">
            <button onclick="loadVideo('video8', 'videoUrl8')">تشغيل</button>
            <iframe id="video8" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <div class="controls">
                <button onclick="togglePlayPause('video8')">إيقاف / تشغيل</button>
                <button class="copy-button" onclick="copyVideoUrl('videoUrl8')">نسخ الرابط</button>
                <label>
                    <input type="checkbox" onchange="toggleLoop('video8', this.checked)">
                    إعادة التشغيل تلقائياً
                </label>
            </div>
        </div>
    </div>

    <div style="text-align: center; margin-top: 40px; color: #777; font-size: 14px;">
        by julian djellouli. Dz
    </div>

    <script>
        var tag = document.createElement('script');
        tag.src = "https://www.youtube.com/iframe_api";
        var firstScriptTag = document.getElementsByTagName('script')[0];
        firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

        let players = {};

        function onYouTubeIframeAPIReady() {
            // يتم إنشاء اللاعبين عند تحميل الفيديو
        }

        function extractVideoId(url) {
            const regex = /(?:youtube\.com\/(?:[^\/]+\/.+\/|(?:v|e(?:mbed)?)\/|.*[?&]v=)|youtu\.be\/)([^"&?\/\s]{11})|youtube\.com\/shorts\/([^"&?\/\s]{11})/;
            const match = url.match(regex);
            return match ? (match[1] || match[2]) : null;
        }

        function loadVideo(iframeId, urlInputId) {
            const url = document.getElementById(urlInputId).value;
            const videoId = extractVideoId(url);
            if (!videoId) {
                alert("الرابط غير صحيح. يرجى التأكد من أنه رابط فيديو يوتيوب.");
                return;
            }
            
            const iframe = document.getElementById(iframeId);
            const loopChecked = document.querySelector(`#${iframeId} + .controls input[type="checkbox"]`).checked;
            const loopParam = loopChecked ? `&loop=1&playlist=${videoId}` : '';

            iframe.src = `https://www.youtube.com/embed/${videoId}?autoplay=1&mute=1${loopParam}`;
            
            if (players[iframeId]) {
                players[iframeId].destroy();
            }
            players[iframeId] = new YT.Player(iframeId);
        }

        function togglePlayPause(videoId) {
            let player = players[videoId];
            if (!player || typeof player.getPlayerState !== 'function') {
                alert("لا يوجد فيديو قيد التشغيل.");
                return;
            }
            
            if (player.getPlayerState() === 1) {
                player.pauseVideo();
            } else {
                player.playVideo();
            }
        }

        function toggleLoop(videoId, shouldLoop) {
            let iframe = document.getElementById(videoId);
            let currentSrc = iframe.src;
            if (!currentSrc) return;

            let url = new URL(currentSrc);
            let videoIdFromUrl = url.pathname.split('/')[2];
            
            if (shouldLoop) {
                url.searchParams.set('loop', '1');
                url.searchParams.set('playlist', videoIdFromUrl);
            } else {
                url.searchParams.delete('loop');
                url.searchParams.delete('playlist');
            }
            iframe.src = url.toString();
        }

        function copyVideoUrl(urlInputId) {
            const urlInput = document.getElementById(urlInputId);
            urlInput.select();
            urlInput.setSelectionRange(0, 99999);
            document.execCommand("copy");
            alert("تم نسخ الرابط!");
        }
    </script>

</body>
</html>
