<template>
  <div class="features1-layout251 thq-section-padding">
    <div class="features1-max-width thq-section-max-width">
      <div class="thq-flex-row features1-section-title">
        <div class="features1-column thq-flex-column">
          <span class="thq-body-small">{{ slogan }}</span>
          <h2 class="thq-heading-2 features1-text1">{{ sectionTitle }}</h2>
        </div>
        <span class="thq-body-small">{{ sectionDescription }}</span>
      </div>
      <div class="features1-content">
        <div class="features1-row thq-flex-row">
          <div class="features1-feature1 thq-flex-column">
            <img
              :alt="feature1ImageAlt"
              :src="feature1ImageSrc"
              class="thq-img-ratio-4-3 features1-feature1-image"
            />
            <div class="features1-content1 thq-flex-column">
              <h3 class="thq-heading-3">{{ feature1Title }}</h3>
              <span class="thq-body-small">{{ feature1Description }}</span>
            </div>
          </div>
          <div class="features1-feature2 thq-flex-column">
            <img
              :alt="feature2ImageAlt"
              :src="feature2ImageSrc"
              class="thq-img-ratio-4-3 features1-feature2-image"
            />
            <div class="features1-content2 thq-flex-column">
              <h3 class="thq-heading-3">{{ feature2Title }}</h3>
              <span class="thq-body-small">{{ feature2Description }}</span>
            </div>
          </div>
          <div class="features1-feature3 thq-flex-column">
            <img
              :alt="feature3ImageAlt"
              :src="feature3ImageSrc"
              class="thq-img-ratio-4-3 features1-feature3-image"
            />
            <div class="features1-content3 thq-flex-column">
              <h3 class="thq-heading-3">{{ feature3Title }}</h3>
              <span class="thq-body-small">{{ feature3Description }}</span>
            </div>
          </div>
        </div>
      </div>
      <div class="features1-actions">
        <button class="thq-button-filled features1-button">
          <span class="thq-body-small">{{ mainAction }}</span>
        </button>
        <button class="thq-button-outline features1-button1">
          <span class="thq-body-small">{{ secondaryAction }}</span>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Features1',
  props: {
    feature2ImageSrc: {
      type: String,
      default:
        'https://images.unsplash.com/photo-1619801629168-3835adcafd74?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w5MTMyMXwwfDF8cmFuZG9tfHx8fHx8fHx8MTcxNjkwMjkwMXw&ixlib=rb-4.0.3&q=80&w=1080',
    },
    feature3ImageSrc: {
      type: String,
      default:
        'https://images.unsplash.com/photo-1497333558196-daaff02b56d0?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w5MTMyMXwwfDF8cmFuZG9tfHx8fHx8fHx8MTcxNjkwMjkwMnw&ixlib=rb-4.0.3&q=80&w=1080',
    },
    feature1Description: {
      type: String,
      default:
        'Engage with your audience and build your brand presence on social media platforms.',
    },
    mainAction: {
      type: String,
      default: 'Learn More',
    },
    feature2Title: {
      type: String,
      default: 'SEO Optimization',
    },
    sectionTitle: {
      type: String,
      default: 'Our Marketing Services',
    },
    feature1ImageAlt: {
      type: String,
      default: 'Social Media Management Image',
    },
    feature2Description: {
      type: String,
      default:
        "Improve your website's visibility on search engines and attract more organic traffic.",
    },
    secondaryAction: {
      type: String,
      default: 'Get Started',
    },
    feature3ImageAlt: {
      type: String,
      default: 'Email Marketing Campaigns Image',
    },
    sectionDescription: {
      type: String,
      default:
        'Explore our range of marketing services tailored to meet your business needs.',
    },
    slogan: {
      type: String,
      default: 'Driving Your Success Through Strategic Marketing',
    },
    feature3Title: {
      type: String,
      default: 'Email Marketing Campaigns',
    },
    feature1ImageSrc: {
      type: String,
      default:
        'https://images.unsplash.com/photo-1541855103-b7d652724617?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w5MTMyMXwwfDF8cmFuZG9tfHx8fHx8fHx8MTcxNjkwMjkwMnw&ixlib=rb-4.0.3&q=80&w=1080',
    },
    feature3Description: {
      type: String,
      default:
        'Reach your target audience effectively through personalized email campaigns.',
    },
    feature2ImageAlt: {
      type: String,
      default: 'SEO Optimization Image',
    },
    feature1Title: {
      type: String,
      default: 'Social Media Management',
    },
  },
}
</script>

<style scoped>
.features1-layout251 {
  width: 100%;
  height: auto;
  display: flex;
  overflow: hidden;
  position: relative;
  align-items: center;
  flex-shrink: 0;
  flex-direction: column;
}
.features1-max-width {
  gap: var(--dl-space-space-threeunits);
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.features1-column {
  gap: var(--dl-space-space-halfunit);
  align-items: flex-start;
  flex-shrink: 0;
}
.features1-content {
  gap: 48px;
  display: flex;
  align-self: stretch;
  align-items: flex-start;
  flex-direction: column;
}
.features1-row {
  align-items: flex-start;
}
.features1-feature1 {
  flex: 1;
}
.features1-content1 {
  align-self: stretch;
  align-items: flex-start;
}
.features1-feature2 {
  flex: 1;
}
.features1-content2 {
  align-self: stretch;
  align-items: flex-start;
}
.features1-feature3 {
  flex: 1;
}
.features1-content3 {
  align-self: stretch;
  align-items: flex-start;
}
.features1-actions {
  gap: var(--dl-space-space-unit);
  display: flex;
  align-items: flex-start;
}
@media(max-width: 991px) {
  .features1-section-title {
    align-items: flex-start;
    flex-direction: column;
  }
  .features1-feature1-image {
    height: 260px;
  }
  .features1-feature2-image {
    height: 260px;
  }
  .features1-feature3-image {
    height: 260px;
  }
}
@media(max-width: 767px) {
  .features1-column {
    width: 100%;
  }
  .features1-text1 {
    text-align: center;
  }
  .features1-row {
    flex-direction: column;
  }
  .features1-feature1-image {
    width: 100%;
  }
  .features1-feature2 {
    width: auto;
  }
  .features1-feature2-image {
    width: 100%;
  }
  .features1-feature3 {
    width: auto;
  }
  .features1-actions {
    flex-wrap: wrap;
  }
}
@media(max-width: 479px) {
  .features1-actions {
    width: 100%;
    flex-direction: column;
  }
  .features1-button {
    width: 100%;
  }
  .features1-button1 {
    width: 100%;
  }
}
</style>
