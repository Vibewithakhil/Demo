#   
<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Dishika - My Haareya ❤️</title>  
    <style>  
        /* [Previous CSS same hai - copy paste mat karo, full code niche] */  
        * { margin: 0; padding: 0; box-sizing: border-box; }  
        body {  
            font-family: 'Segoe UI', sans-serif;  
            background: linear-gradient(135deg, #ff6b9d, #4ecdc4, #667eea);  
            background-size: 400% 400%;  
            animation: gradientShift 10s ease infinite;  
            min-height: 100vh; display: flex; align-items: center; justify-content: center;  
        }  
        /* [Sab same CSS - space bachane ke liye short kiya] */  
    </style>  
</head>  
<body>  
    <div class="container">  
        <!-- ✅ DISHIKA PHOTO -->  
        <img src="https://i.postimg.cc/gcvMfBtr/2c058fa4-4d93-4f67-939c-7becc3efbba9.jpg"   
             alt="Dishika" class="profile-pic" onclick="zoomPhoto()">  
          
        <h1>Dishika - My Haareya ❤️</h1>  
          
        <div class="typing-container">  
            <span class="typing-text">  
                See dekh baby 😏 Hamesha thank you bolta rahunga ki meri life me aayi 💕  
            </span>  
        </div>  
          
        <!-- 🎵 HAAREYA VOICE NOTE - TUMHARA LINK ✅ -->  
        <div class="voice-note" onclick="playHaareya()">  
            <div class="play-btn">🎶</div>  
            <div class="voice-text">Play Haareya for my baby...</div>  
        </div>  
          
        <!-- 💌 ROMANTIC MEMORIES -->  
        <div class="confession-card" id="loveMsg" style="opacity:0;">  
            Har roz itna sukoon diya. Pehli baar hath pakadne ka feel,   
            kandhe pe sone wala moment, first kiss ka heavenly touch,   
            Uttam Nagar wala cute hug - har baar butterflies udte hai dil me.  
            <div class="signature">~ your uduu bby' 🫠✨</div>  
        </div>  
          
        <!-- 🎼 HAAREYA LYRICS -->  
        <div class="lyrics-card" id="haareyaLyrics">  
            <strong>O Hareya Main Dil Haareya 🎶</strong><br><br>  
            Dekheya main chand dekheya<br>  
            Nooran wale sitare dekheya<br>  
            <em>Par tere jaisa na koi dekheya</em><br><br>  
            Lagta hai nigahon mein teri<br>  
            Bin dube rehna hi nahi<br>  
            <strong>Main haara tujhpe... oo</strong>  
        </div>  
          
        <div class="footer">Made with ∞ love for my Haareya 🌹</div>  
    </div>  
  
    <!-- 🎤 TUMHARA ACTUAL VOICE NOTE LINK ✅ -->  
    <audio id="haareyaAudio" src="https://files.catbox.moe/7c0j1g.m4a" preload="auto"></audio>  
  
    <!-- [JavaScript same - play function ready] -->  
    <script>  
        function playHaareya() {  
            const audio = document.getElementById('haareyaAudio');  
            audio.play().then(() => {  
                document.querySelector('.voice-note').innerHTML =   
                '<div class="play-btn">⏸️</div><div class="voice-text">Haareya playing for Dishika...</div>';  
                setTimeout(() => {  
                    document.getElementById('loveMsg').style.opacity = '1';  
                }, 1000);  
            }).catch(e => {  
                alert('Voice note download karke suno meri Haareya 🎧');  
            });  
        }  
    </script>  
</body>  
</html>  
