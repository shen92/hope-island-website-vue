<template>
  <div class="about">
    <SectionAlt backgroundPath="/images/scenes/level3b.jpg">
      <div class="title heroTitle textLight">Welcome to Hope Island</div>
    </SectionAlt>
    <Introduction/>
    <VideoPlayer src="https://www.youtube.com/embed/kx65PHULkig?controls=0"/>
    <SectionAlt backgroundPath="/images/scenes/level2-2.jpg">
      <div style="display: flex; flex-direction: column; align-items: center">
        <div class="title heroTitle textLight">Design and Inspirations</div>
        <div class="title heroSubTitle textLight" style="margin-top: 2vh">Read More on <span><a class="link" href="/files/Hope_Island_GDD.pdf" download>Game Design Document</a></span></div>
      </div>
    </SectionAlt>
    <Inspirations/>
    <SectionAlt backgroundPath="/images/scenes/level1b.jpg">
      <div class="title heroTitle textLight">Gameplay and Mode</div>
    </SectionAlt>
    <GameMode/>
    <SectionAlt backgroundPath="/images/characters/charlottel1.jpg">
      <div class="title heroTitle textLight">Characters and Skills</div>
    </SectionAlt>
    <Characters/>
    <SectionAlt backgroundPath="/images/scenes/level1-2.jpg">
      <div class="title heroTitle textLight">Maps and Levels</div>
    </SectionAlt>
    <Section backgroundPath="/images/scenes/level0.jpg" :isReversed="false">
      <div class="slotContentContainer map">
        <div class="slotContent">
          <div>
            <div class="title cardTitle">Walnut Town</div>
            <div class="subtitle cardSubTitle">Where adventure begins</div>
          </div>
          <div style="width: 25vw">
            <div class="content cardContent" >
              Walnut Town is a beautiful and quiet town in the heart of Wild Timberland. It is also the safe-house of Vincent, Marc and Charlotte.
            </div>
          </div>
        </div>
      </div>
    </Section>
    <Section backgroundPath="/images/scenes/level1-4.jpg" :isReversed="true">
      <div class="slotContentContainer map">
        <div class="slotContent">
          <div>
            <div class="title cardTitle">Wild Timberland</div>
            <div class="subtitle cardSubTitle">Peaceful but dangerous</div>
          </div>
          <div style="width: 25vw">
            <div class="content cardContent" >
              Wild Timberland possesses the wildest the most ancient forest on hope island. This area owns an amazing landscape with forest, valleys, rivers and lakes. There also exists lots of danger.
            </div>
          </div>
        </div>
      </div>
    </Section>
    <Section backgroundPath="/images/scenes/level2-1.jpg" :isReversed="false">
      <div class="slotContentContainer map">
        <div class="slotContent">
          <div>
            <div class="title cardTitle">Barren Desert</div>
            <div class="subtitle cardSubTitle">Hot, dry and mysterious</div>
          </div>
          <div style="width: 25vw">
            <div class="content cardContent" >
              The Barren Desert is the hottest and driest place on Hope Island. In the Barren Desert, there are villages, oases and ancient relics. Be careful, don't get lost in the Barren Desert.
            </div>
          </div>
        </div>
      </div>
    </Section>
    <Section backgroundPath="/images/scenes/level3-1.jpg" :isReversed="true">
      <div class="slotContentContainer map">
        <div class="slotContent">
          <div>
            <div class="title cardTitle">Harbor Town</div>
            <div class="subtitle cardSubTitle">Harbor Town</div>
          </div>
          <div style="width: 25vw">
            <div class="content cardContent" >
              Harbor Town is the most important town on Hope Island. It used to be busy and prosperous, but now it has been occupied by the Matard Soldiers.
            </div>
          </div>
        </div>
      </div>
    </Section>
    <Footer/>
  </div>
</template>

<script>
import { Section, SectionAlt, Introduction, VideoPlayer, Inspirations, GameMode, Characters, Footer } from '@/components'

export default {
  name: 'About',
  components: {
    Footer,
    Section,
    SectionAlt,
    Introduction,
    VideoPlayer,
    Inspirations,
    GameMode,
    Characters
  },
}
</script>

<style lang="scss" scoped>
  .about {
    height: 100%;
    display: flex;
    flex-direction: column;
  }

  .heroTitle {
    font-size: 60px;
  }

  .heroSubTitle {
    font-size: 32px;
  }

  .slotContentContainer {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
  }

  .slotContent {
    margin-left: 20%;
    width: fit-content;
    display: flex;
    flex-direction: column;
    gap: 8vh;
  }

  .cardTitle {
    font-size: 40px;
  }

  .cardSubTitle {
    font-size: 20px;
  }

  .cardContent {
    font-size: 20px;
    display: flex;
  }

  .map {
    background: #FAF3DD 0% 0% no-repeat padding-box;
  }

</style>