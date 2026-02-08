# naman-sharma55
this is my 12th repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Messenger Style UI</title>
    <style>
        :root {
            --messenger-blue: #0084ff;
            --bg-grey: #f0f0f0;
            --bubble-grey: #e4e6eb;
        }

        body {
            font-family: 'Segoe UI', Helvetica, Arial, sans-serif;
            background-color: #f9f9f9;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        /* App Container */
        .messenger-window {
            width: 100%;
            max-width: 400px;
            height: 600px;
            background: white;
            display: flex;
            flex-direction: column;
            box-shadow: 0 12px 28px rgba(0,0,0,0.1);
            border-radius: 12px;
            overflow: hidden;
        }

        /* Header */
        .header {
            padding: 10px 15px;
            display: flex;
            align-items: center;
            border-bottom: 1px solid #ddd;
            gap: 12px;
        }

        .avatar {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: #ddd;
        }

        .user-status {
            flex-grow: 1;
        }

        .user-status b { display: block; font-size: 15px; }
        .user-status span { font-size: 12px; color: #65676B; }

        /* Chat Area */
        .chat-area {
            flex: 1;
            padding: 15px;
            overflow-y: auto;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        /* Bubbles */
        .bubble {
            max-width: 70%;
            padding: 10px 14px;
            border-radius: 18px;
            font-size: 14px;
            line-height: 1.4;
        }

        .incoming {
            align-self: flex-start;
            background-color: var(--bubble-grey);
            color: black;
        }

        .outgoing {
            align-self: flex-end;
            background-color: var(--messenger-blue);
            color: white;
        }

        /* Video Bubble */
        .video-bubble {
            width: 100%;
            border-radius: 15px;
            overflow: hidden;
            margin-bottom: 5px;
        }

        .video-bubble iframe {
            width: 100%;
            aspect-ratio: 1 / 1; /* Square for Messenger style */
            border: none;
            display: block;
        }

        /* Footer */
        .footer {
            padding: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .input-pill {
            flex: 1;
            background: var(--bg-grey);
            padding: 8px 15px;
            border-radius: 20px;
            color: #8a8d91;
            font-size: 14px;
        }

        .like-icon {
            color: var(--messenger-blue);
            font-size: 22px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <div class="messenger-window">
        <div class="header">
            <div class="avatar"></div>
            <div class="user-status">
                <b>SSB Prep Group</b>
                <span>Active 5m ago</span>
            </div>
            <span style="color: var(--messenger-blue); font-size: 20px;">📞</span>
        </div>

        <div class="chat-area">
            <div class="bubble incoming">Hey! Have you seen this video on the Indian Navy TES entry?</div>

            <div class="bubble outgoing">
                <div class="video-bubble">
                    <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0" title="Video preview"></iframe>
                </div>
                Just watching it now. Very helpful for the interview!
            </div>
        </div>

        <div class="footer">
            <span style="font-size: 20px; color: #65676B;">➕</span>
            <div class="input-pill">Aa</div>
            <span class="like-icon">👍</span>
        </div>
    </div>

</body>
</html>
