<template>
  <div>
    <TheBanner image="/images/banners/PWFeb15Cartwright-frontis-hero.jpg">
      <h1 class="banner-title">Анализ и диагностика причин неудовлетворительной производительности систем на базе ПО Oracle</h1>
      <span class="banner-subtitle">Выполнение работ по настройке производительности, от диагностики и рекомендаций до внедрения исправлений.</span>
    </TheBanner>
    <div class="container-fluid bg-molecular-pattern">
      <div class="container py-30">
        <FeaturesList :items="featuresList" />
      </div>
    </div>
    <div class="container-fluid bg-neutral-primary">
      <div class="container py-60">
        <FeaturesCard
          v-for="(featuresCard, index) in featuresCards"
          :key="index"
          :title="featuresCard.title"
          :content="featuresCard.content"
        ></FeaturesCard>
      </div>
    </div>
  </div>
</template>

<script>
  import TheBanner from '~/components/base/TheBanner.vue'
  import FeaturesList from '~/components/base/FeaturesList.vue'
  import FeaturesCard from '~/components/base/FeaturesCard.vue'

  export default {
    name: "oracle",
    components: {
      TheBanner, FeaturesList, FeaturesCard
    },
    data() {
      return {
        featuresList: [
          {icon: 'qrcode', content: 'Консультационная помощь и выполнение работ у Клиента по установке и конфигурированию операционных систем и программного обеспечения Oracle для его оптимально производительной работы.'},
          {icon: 'solution', content: 'Инсталляция высокодоступных и надежных решений на базе технологии Real Application Clusters, Oracle Data Guard, GoldenGate.'},
          {icon: 'setting', content: 'Настройка оптимальных процедур резервного копирования и восстановления баз данных Oracle либо предоставление рекомендаций по его настройке.'},
          {icon: 'table', content: 'Межплатформенная миграция баз данных Oracle, настройки совместимости приложений, помощь с апргрейдом версий.'},
          {icon: 'upload', content: 'Установка и рекомендации по настройке систем управления и мониторинга на базе Grid Control и Oracle Enterprise Manager.'},
          {icon: 'share-alt', content: 'Помощь с восстановлением баз данных Oracle после аварийных ситуаций, помощь с извлечением данных.'},
          {icon: 'team', content: 'Настройка и консультации по гетерогенным сервисам Oracle GoldenGate.'},
          {icon: 'profile', content: 'Настройка и консультации по ПО Oracle TimesTen.'},
          {icon: 'file-sync', content: 'Выполнение работ по администрированию баз данных Oracle , непосредственно на площадке Клиента, по телефону либо удаленно, в течение предусмотренного контрактом времени. '},
        ],
        featuresCards: [
          { title: 'Бесплатная услуга – поверхностное знакомство с системой', content: '<ul><li>Наши специалисты выезжают на площадку клиента.</li><li>В рамках диалога с клиентом выясняют моменты на которые больше всего жалуется заказчик.</li><li>Делают обследование заявленных заказчиком мест системы и выносят заключение о возможности ее оптимизации.</li></ul>'},
          { title: 'Аудит системы заказчика', content: '<ul><li>Наши специалисты выезжают на площадку клиента.</li><li>В рамках диалога с клиентом выясняют моменты на которые больше всего жалуется заказчик и начинают аудит с поиска способов оптимизации в указанных заказчиком модулях ПО.</li><li>Делают комплексное обследование всех узких мест системы и выносят заключение о возможности ее оптимизации.</li><li>В акте аудита мы указываем программные модули, процедуры, функции, запросы требующие первоначального тюнинга. Рекомендации выдаются специалистам заказчика и применяются им.</li></ul>' },
          { title: 'Услуга по администрированию СУБД Oracle и оптимизации прикладного кода в режиме 8*5', content: '<ul><li>Клиент получает поддержку в течение стандартного рабочего времени с 9-30 до 18-00 c понедельника по пятницу, по вопросам производительности его системы, по вопросам администрирования его системы и по любым вопросам связанным с продуктами компании Oracle. Поддержка осуществляется как удаленно через сайт поддержки, по телефону, так и с присутствием экспертов на площадке заказчика.</li><li>Цена зависит от количества систем и продуктов, по которым необходимо получать консультации. </li></ul><p>Администраторы oracle предоставляемые компанией обладают сертификатами:</p><ul><li>Oracle certified master</li><li>Oracle tuning expert</li><li>Oracle real application cluster expert</li></ul><p>Аудит включен в стоимость услуги и выполняется ежеквартально.</p>' },
          { title: 'Услуга по администрированию и оптимизации СУБД Oracle и оптимизации прикладного кода в режиме 24*7', content: '<ul><li>Клиент получает поддержку в течение стандартного рабочего времени с 9-30 до 18-00 c понедельника по пятницу, по вопросам производительности его системы, по вопросам администрирования его системы и по любым вопросам связанным с продуктами компании Oracle. Поддержка осуществляется как удаленно через сайт поддержки, по телефону, так и с присутствием экспертов на площадке заказчика.</li><li>Цена зависит от количества систем и продуктов, по которым необходимо получать консультации. </li></ul><p>Администраторы oracle предоставляемые компанией обладают сертификатами:</p><ul><li>Oracle certified master</li><li>Oracle tuning expert</li><li>Oracle real application cluster expert</li></ul><p>Аудит включен в стоимость услуги и выполняется ежеквартально.</p>' },

        ]
      }
    }

  }
</script>

<style>

</style>
