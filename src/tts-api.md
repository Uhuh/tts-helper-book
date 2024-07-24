# TTS API

## If you're using a tool like MixItUp

This is the perfect thing to use! Because currently **TTS Helper** doesn't support **YouTube**, you can use **MixItUp** to send TTS request here.

**TTS Helper** is lacking severely in it's exposed APIs, not that it needs much to begin with!

There's currently only one exposed API endpoint.    

All this does is allows you to send TTS request to **TTS Helper**
If the username is in a block list, or if the text content contains a banned word, your request will be ignored.

Here's the info:
<head>
  <title>HTML Table</title>
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
    <th>Data Structure</th>
  </tr>
  <tr>
    <td>POST</td>
    <td>http://localhost:12589/tts</td>
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
</table>

All of these can be changed, obviously, besides the `platform` field.   
Currently `platform` supports `twitch`, `youtube` and `vstream` (rip)