---
title: "Страница 1"
image: "/books/cat-story/images/page-01.jpg"
audio_kz: "/books/cat-story/audio/page-01-kz.mp3"
audio_en: "/books/cat-story/audio/page-01-en.mp3"
text_kz: "Қыз бен мысық далаға шықты."
text_en: "The girl and the cat went outside."
---

# Страница 1

![Иллюстрация]({{ .Params.image }})

**Казахский:** {{ .Params.text_kz }}  
**English:** {{ .Params.text_en }}

<button onclick="play('kz')">Озвучить на казахском</button>
<button onclick="play('en')">Play in English</button>

<audio id="audio-kz"><source src="{{ .Params.audio_kz }}"></audio>
<audio id="audio-en"><source src="{{ .Params.audio_en }}"></audio>

<script>
function play(l) {
  document.getElementById('audio-' + l).play();
}
</script>
