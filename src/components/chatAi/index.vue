<template>
    <div class="app-container">
      <SideNavigation />
      <SearchHeader />
      <div class="main-content">
        <div class="content-area">
          <AssistantIntro />
          <!-- <div class="feature-cards">
            <div class="cards-row">
              <NewsCard />
              <ToolsCard />
              <CodeCard />
            </div>
            <div class="cards-row">
              <TranslationCard />
              <PresentationCard />
              <FontCard />
            </div>
          </div> -->
          <contentList />
        </div>
        <FooterActions />
      </div>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  import SideNavigation from './SideNavigation.vue'
  import SearchHeader from './SearchHeader.vue'
  import AssistantIntro from './AssistantIntro.vue'
  import NewsCard from './cards/NewsCard.vue'
  import ToolsCard from './cards/ToolsCard.vue'
  import CodeCard from './cards/CodeCard.vue'
  import TranslationCard from './cards/TranslationCard.vue'
  import PresentationCard from './cards/PresentationCard.vue'
  import FontCard from './cards/FontCard.vue'
  import FooterActions from './FooterActions.vue'
  import contentList from './contentList.vue'
  </script>
  
  <style>
  :root {
    --primary-color: #6366f1;
    --sidebar-bg: #6366f1;
    --card-bg: #f9fafb;
    --hover-bg: #f3f4f6;
    --border-color: #e5e7eb;
    --text-primary: #111827;
    --text-secondary: #4b5563;
  }
  
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'PingFang SC', 'Microsoft YaHei', sans-serif;
  }
  
  .app-container {
    display: flex;
    height: 100vh;
    width: 100%;
    overflow: hidden;
  }
  
  .main-content {
    flex: 1;
    display: flex;
    flex-direction: column;
    overflow: hidden;
  }
  
  .content-area {
    flex: 1;
    /* margin: 20px; */
    overflow-y: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .feature-cards {
    width: 100%;
    max-width: 1200px;
    margin-top: 20px;
  }
  
  .cards-row {
    display: flex;
    gap: 16px;
    margin-bottom: 16px;
    flex-wrap: wrap;
  }
  
  @media (max-width: 768px) {
    .cards-row {
      flex-direction: column;
    }
  }
  </style>