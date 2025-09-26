# Patan-news-
No filter only truth the fourth stambh start the breaking news to solve problems 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Patan Local News</title>
    <style>
        body { font-family: Arial, sans-serif; margin:0; padding:0; background-color:#f4f4f4; }
        header { background-color:#2c3e50; color:white; padding: 15px 20px; text-align:center; }
        nav { background-color:#34495e; padding:10px 20px; }
        nav a { color:white; margin:0 15px; text-decoration:none; }
        nav a:hover { text-decoration:underline; }
        .container { max-width:1200px; margin:20px auto; padding:0 20px; }
        .news-card { background:white; padding:15px; margin-bottom:20px; border-radius:8px; box-shadow:0 2px 5px rgba(0,0,0,0.1); }
        .news-card h2 { margin-top:0; color:#2c3e50; }
        .news-card p { color:#555; }
        footer { background-color:#2c3e50; color:white; text-align:center; padding:15px; margin-top:20px; }
        .add-news { background:white; padding:15px; margin-bottom:20px; border-radius:8px; box-shadow:0 2px 5px rgba(0,0,0,0.1); }
        input, textarea { width:100%; padding:10px; margin:5px 0; border-radius:5px; border:1px solid #ccc; }
        button { padding:10px 20px; background-color:#2c3e50; color:white; border:none; border-radius:5px; cursor:pointer; }
        button:hover { background-color:#34495e; }
    </style>
</head>
<body>
    <header>
        <h1>Patan Local News</h1>
        <p>ताज़ा समाचार और लोकल इवेंट्स</p>
    </header>
    <nav>
        <a href="#">होम</a>
        <a href="#">राजनीति</a>
        <a href="#">संस्कृति</a>
        <a href="#">खेल</a>
        <a href="#">इवेंट्स</a>
        <a href="#">संपर्क</a>
    </nav>
    <div class="container">
        <div class="add-news">
            <h2>न्यूज़ जोड़ें</h2>
            <input type="text" id="news-title" placeholder="न्यूज़ का शीर्षक">
            <textarea id="news-content" rows="4" placeholder="न्यूज़ की सामग्री"></textarea>
            <button onclick="addNews()">जोड़ें</button>
        </div>
        <div id="news-list">
            <div class="news-card">
                <h2>स्थानीय पंचायत में नयी योजनाओं की घोषणा</h2>
                <p>पाटन ब्लॉक की पंचायत ने किसानों के लिए नई सब्सिडी योजनाओं की घोषणा की। किसानों को अब अधिक सुविधाएं उपलब्ध होंगी।</p>
            </div>
            <div class="news-card">
                <h2>ग्राम उत्सव 2025 की तैयारियां शुरू</h2>
                <p>पाटन ब्लॉक के सभी गांवों में अगले महीने होने वाले उत्सव की तैयारियां जोर-शोर से चल रही हैं।</p>
            </div>
            <div class="news-card">
                <h2>स्थानीय खेल प्रतियोगिता का आयोजन</h2>
                <p>स्कूल और कॉलेज स्तर की खेल प्रतियोगिता पाटन के खेल मैदान में आयोजित की जा रही है। सभी युवाओं को आमंत्रित किया गया है।</p>
            </div>
        </div>
    </div>
    <footer>
        <p>&copy; 2025 Patan Local News. सभी अधिकार सुरक्षित।</p>
    </footer>

    <script>
        function addNews() {
            var title = document.getElementById('news-title').value;
            var content = document.getElementById('news-content').value;
            if(title && content) {
                var newsList = document.getElementById('news-list');
                var newsCard = document.createElement('div');
                newsCard.className = 'news-card';
                newsCard.innerHTML = '<h2>' + title + '</h2><p>' + content + '</p>';
                newsList.prepend(newsCard);
                document.getElementById('news-title').value = '';
                document.getElementById('news-content').value = '';
            } else {
                alert('कृपया शीर्षक और सामग्री दोनों दर्ज करें।');
            }
        }
    </script>
</body>
</html> .html 
