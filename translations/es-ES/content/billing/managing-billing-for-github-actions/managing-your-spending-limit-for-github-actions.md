---
title: Administración del límite de gasto para las acciones de GitHub
intro: 'Puedes configurar un límite de gastos para el uso de {% data variables.product.prodname_actions %}.'
redirect_from:
  - /github/setting-up-and-managing-billing-and-payments-on-github/managing-your-spending-limit-for-github-actions
  - /github/setting-up-and-managing-billing-and-payments-on-github/managing-billing-for-github-actions/managing-your-spending-limit-for-github-actions
versions:
  fpt: '*'
  ghec: '*'
type: how_to
topics:
  - Actions
  - Enterprise
  - Organizations
  - Spending limits
  - User account
shortTitle: Spending limits for Actions
ms.openlocfilehash: c1bd595a866b9e48fa4e82ebe93718328514fad9
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/05/2022
ms.locfileid: '145091705'
---
## Acerca de los límites de gastos para {% data variables.product.prodname_actions %}

{% data reusables.actions.actions-billing %}

{% data reusables.actions.actions-spending-limit-brief %}

{% data reusables.actions.actions-packages-set-spending-limit %} Para más información sobre los precios del uso de {% data variables.product.prodname_actions %}, vea "[Acerca de la facturación de {% data variables.product.prodname_actions %}](/billing/managing-billing-for-github-actions/about-billing-for-github-actions)".

{% ifversion ghec %} Si ha comprado {% data variables.product.prodname_enterprise %} mediante un Acuerdo de Microsoft Enterprise, puede conectar el id. de la suscripción de Azure a la cuenta empresarial para habilitar y pagar por el uso de {% data variables.product.prodname_actions %} más allá de las cantidades que se incluyen en la cuenta. Para más información, vea "[Conexión de una suscripción de Azure a la empresa](/billing/managing-billing-for-your-github-account/connecting-an-azure-subscription-to-your-enterprise)".
{% endif %}

Tan pronto como configures un límite de gastos diferente a $0, serás responsable de cualquier uso excedente que se suscite en el periodo de facturación actual. Por ejemplo, si tu organización utiliza {% data variables.product.prodname_team %}, no permite excedentes, y crea artefactos de flujo de trabajo que incrementan tu uso de almacenamiento para el mes en curso de 1.9GB a 2.1GB, utilizarás un poco más de almacenamiento que los 2Gb incluidos en tu producto.

Ya que no has habilitado los excedentes, tu siguiente intento de crear un artefacto de un flujo de trabajo fallará. No recibirás una cuenta por esos 0.1GB extras en ese mes. Sin embargo, si habilitas los excedentes, tu primer factura incluirá el excedente de 0.1GB del ciclo de facturación actual, así como cualquier otro excedente que acumules.

## Administrar el límite de gasto de {% data variables.product.prodname_actions %} para tu cuenta personal

Cualquiera puede administrar el límite de gasto de {% data variables.product.prodname_actions %} para su propia cuenta personal.

{% data reusables.user-settings.access_settings %} {% data reusables.user-settings.billing_plans %} {% data reusables.dotcom_billing.manage-spending-limit %} {% data reusables.dotcom_billing.monthly-spending-limit %} {% data reusables.dotcom_billing.update-spending-limit %}

## Administrar el límite de gastos de {% data variables.product.prodname_actions %} para tu organización

Los propietarios de las organizaciones pueden administrar el límite de gastos de {% data variables.product.prodname_actions %} para una organización.

{% data reusables.organizations.billing-settings %} {% data reusables.dotcom_billing.manage-spending-limit %} {% data reusables.dotcom_billing.monthly-spending-limit-actions-packages %} {% data reusables.dotcom_billing.update-spending-limit %}

{% ifversion ghec %}
## Administrar el límite de gastos de {% data variables.product.prodname_actions %} para tu cuenta empresarial

Los propietarios de la empresa y gerentes de facturación pueden administrar el límite de gastos para {% data variables.product.prodname_actions %} para una cuenta empresarial.

{% data reusables.enterprise-accounts.access-enterprise %} {% data reusables.enterprise-accounts.settings-tab %} {% data reusables.enterprise-accounts.billing-tab %}
1. Encima de "Uso mensual de {% data variables.product.prodname_actions %} y paquetes", haga clic en **Límite de gasto**.
  ![Pestaña Límite de gasto](/assets/images/help/settings/spending-limit-tab-enterprise.png) {% data reusables.dotcom_billing.monthly-spending-limit %} {% data reusables.dotcom_billing.update-spending-limit %} {% endif %}

## Administrar las notificaciones de uso y límite de gastos
{% data reusables.billing.email-notifications %}
