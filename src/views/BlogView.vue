<template>
    <main>
        <section>
            <div class="blog-card">
                <div class="blog-card-photo"></div>
                <div class="blog-card-abstract">
                    <h2><RouterLink to="/blogPosts/HuxleyBrothers">Příběh bratří Huxleyů, aneb co je to Transhumanismus, a proč by mě to mělo zajímat?</RouterLink></h2>
                    <div class="article-details">
                        <p>Autor: Martin Kadlec</p>
                        <p>Datum publikace: <time datetime="2024-11-5">5.11.2024</time></p>
                        <p>Naposledy aktualizováno: <time datetime="2024-11-17">17.11.2024</time></p>
                    </div>
                    <p>
                        Dvacáté století přineslo světu mnoho dobrého i špatného. Napozadí nejrychlejšího kulturního a technologického vývoje naší historie dva
                        bratři z anglické aristokracie víceméně omylem položili základ filozofického směru, který se dnes tiše promítá do modeního vývoje IT, geopolitiky,
                        zdravotnictví a mnohého dalšího - a zároveň definovali jeho fundamentální dualitu. Gather round, dnes vyprávím příběh bratří Huxleyů a vysvětlím, proč je pro nás důležitý.
                    </p>
                </div>
            </div>
        </section>
    </main>
</template>


<style scoped>
.article-details{
  border-top: 1px solid var(--color-border);
  border-bottom: 1px solid var(--color-border);;
  margin: 0.5rem 0;
}

.article-details p {
  display: inline-block;
  margin: 0 5px;
}
</style>