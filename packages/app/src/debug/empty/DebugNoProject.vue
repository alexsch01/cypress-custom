<template>
  <DebugEmptyView
    :title="t('debugPage.emptyStates.debugDirectlyInCypress')"
    :description="t('debugPage.emptyStates.reviewRerunAndDebug')"
    :example-test-name="t('debugPage.emptyStates.noProjectTestMessage')"
    :help-link-text="t('debugPage.emptyStates.learnAboutProjectSetup')"
    help-link-href="https://on.cypress.io/adding-new-project"
  >
    <template #cta>
      <CloudConnectButton utm-medium="Debug Tab" />
    </template>
  </DebugEmptyView>
</template>

<script lang="ts" setup>
import DebugEmptyView from './DebugEmptyView.vue'
import { useI18n } from '@cy/i18n'
import CloudConnectButton from '../../runs/CloudConnectButton.vue'

const { t } = useI18n()

</script>
