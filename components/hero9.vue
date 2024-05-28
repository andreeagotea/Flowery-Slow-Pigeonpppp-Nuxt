<template>
  <div class="hero9-header30 thq-section-padding">
    <img :alt="image1Alt" :src="image1Src" class="hero9-image" />
    <div class="hero9-container"></div>
    <div class="hero9-max-width thq-section-max-width">
      <div class="hero9-content">
        <h1 class="hero9-text thq-heading-1">{{ heading1 }}</h1>
        <p class="hero9-text1 thq-body-large">{{ content1 }}</p>
        <div class="hero9-actions">
          <button class="thq-button-filled hero9-button">
            <span class="hero9-text2 thq-body-small">{{ action1 }}</span>
          </button>
          <button class="thq-button-outline hero9-button1">
            <span class="hero9-text3 thq-body-small">{{ action2 }}</span>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hero9',
  props: {
    content1: {
      type: String,
      default:
        'Explore our range of marketing services to help your business grow',
    },
    action1: {
      type: String,
      default: 'Learn More',
    },
    heading1: {
      type: String,
      default: 'Welcome to our Marketing Services Website',
    },
    image1Alt: {
      type: String,
      default: 'Marketing Services Image',
    },
    action2: {
      type: String,
      default: 'Get in touch',
    },
    image1Src: {
      type: String,
      default:
        'https://images.unsplash.com/photo-1504598561342-6b76820ef3e6?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w5MTMyMXwwfDF8cmFuZG9tfHx8fHx8fHx8MTcxNjkwMjkwMXw&ixlib=rb-4.0.3&q=80&w=1080',
    },
  },
}
</script>

<style scoped>
.hero9-header30 {
  gap: var(--dl-space-space-twounits);
}
.hero9-image {
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  position: absolute;
  object-fit: cover;
}
.hero9-container {
  top: 0px;
  left: 0px;
  right: 0px;
  width: 100%;
  bottom: 0px;
  height: 100%;
  display: flex;
  position: absolute;
  align-items: flex-start;
  flex-direction: column;
  background-color: rgba(255,255,255,0.7);
}
.hero9-max-width {
  gap: var(--dl-space-space-oneandhalfunits);
  width: 100%;
  display: flex;
  z-index: 1;
  align-items: center;
  flex-direction: column;
}
.hero9-content {
  gap: var(--dl-space-space-oneandhalfunits);
  display: flex;
  align-self: stretch;
  align-items: center;
  flex-direction: column;
}
.hero9-text {
  text-align: center;
}
.hero9-text1 {
  text-align: center;
}
.hero9-actions {
  gap: var(--dl-space-space-unit);
  display: flex;
  align-items: flex-start;
}
.hero9-text2 {
  text-align: center;
}
.hero9-text3 {
  text-align: center;
}
@media(max-width: 991px) {
  .hero9-text {
    text-align: center;
  }
  .hero9-text1 {
    text-align: center;
  }
}
@media(max-width: 479px) {
  .hero9-actions {
    width: 100%;
    flex-direction: column;
  }
  .hero9-button {
    width: 100%;
  }
  .hero9-button1 {
    width: 100%;
  }
}
</style>
