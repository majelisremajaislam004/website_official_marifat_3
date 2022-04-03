<template>
    <main>
        <div class="container">
            <h2 class="header text-center">APA ITU MA'RIFAT ?</h2>
            <p>Jadi<abbr title="Majelis Remaja Islam SMKN 4 Tasikmalaya"> MA'RIFAT</abbr> Suatu Organisasi Keagamaan di SMKN 4 Tasikmalaya yang Mewadahi siswa/i yang sangat ingin memperdalam lagi ilmu agama karena keterbatasan jam mata pelajaran <abbr title="Pendidikan Agama Islam"> PAI</abbr> di sekolah.</p>
            <p>Bahkan sekarang<abbr title="Majelis Remaja Islam SMKN 4 Tasikmalaya"> MA'RIFAT</abbr> dikenal sebagai induk dari dua organisasi keagamaan di SMKN 4 Tasikmalaya mencakup <abbr title="Rohani Islam">Rohis</abbr> dan <abbr title="Ikatan Remaja Mesjid">IRMA</abbr>, sehingga menjadikan MA'RIFAT sangat disegani dan diminati oleh siswa/i.</p>
            <p>Untuk mengenal lebih jauh lagi mari kita mulai membahasnya, simak penjelasan berikut ;</p>
        </div>
    </main>
</template>


<style lang="scss" scoped>
body {
  font-family: 'Roboto', sans-serif;
  font-size: 1.3rem;
}

.container {
  line-height: 1.5;
  margin: 1rem;
  padding: 40px 25px;
}

abbr {
  position: relative;
  text-decoration: none;
}

abbr:hover::after {
  background: #add8e6;
  border-radius: 4px;
  bottom: 100%;
  content: attr(title);
  display: block;
  left: 100%;
  padding: 1em;
  position: absolute;    
  width: 280px;
  z-index: 1;
}
</style>
