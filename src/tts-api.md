# TTS API

TTS Helper has a bare bones API.

If you have software that can send request out, you can trigger certain TTS Helper features with them.

> TTS Helper's API listens for request here: `http://localhost:12589`

Currently `platform` supports `twitch`, `youtube`. If you pass an unknown platform, we'll render a `?`

<head>
  <title>API Table</title>
  <style>
    table {
      width: 100%;
    }
  </style>
</head>
<body>

<table>
  <tr>
    <th>HTTP Type</th>
    <th>EndPoint</th>
    <th>Body</th>
  </tr>
  <tr>
    <td>POST</td>
    <td><code style="white-space: nowrap">/tts</code></td>
    <td>
      <pre>
        {
            "username": "Panku",
            "platform": "twitch",
            "text": "Hello world!",
            "char_limit": 300
        }
      </pre>
    </td>
  </tr>
  <tr>
    <td>POST</td>
    <td><code style="white-space: nowrap">/toggle-pause-status</code></td>
    <td>
      No body for this request.
    </td>
  </tr>
  <tr>
    <td>POST</td>
    <td><code style="white-space: nowrap">/skip-current-playing</code></td>
    <td>
      No body for this request.
    </td>
  </tr>
  <tr>
    <td>POST</td>
    <td><code style="white-space: nowrap">/ai-tts</code></td>
    <td>
      <pre>
        {
            "username": "Panku",
            "platform": "twitch",
            "text": "How're you?",
            "char_limit": 300
        }
      </pre>
    </td>
  </tr>
  <tr>
    <td>POST</td>
    <td><code style="white-space: nowrap">/ai-response</code></td>
    <td>
      <pre>
        {
            "username": "Panku",
            "platform": "twitch",
            "text": "How're you?",
            "char_limit": 300
        }
      </pre>
    </td>
  </tr>
  <tr>
    <td>POST</td>
    <td><code style="white-space: nowrap">/react-ai-image</code></td>
    <td>
      <pre>
        {
            "text": "What do you see?",
            "image": "*B64 encoded image here*"
        }
      </pre>
    </td>
  </tr>
  <tr>
    <td>POST</td>
    <td><code style="white-space: nowrap">/trigger-ai-vision</code></td>
    <td>
      <pre>
        {
            "username": "Panku",
            "platform": "twitch",
            "text": "What do you see?",
            "char_limit": 300
        }
      </pre>
    </td>
  </tr>
</table>