---
title: Descargar los artefactos del flujo de trabajo
intro: Puedes descargar artefactos archivados antes de que venzan automáticamente.
product: '{% data reusables.gated-features.actions %}'
versions:
  free-pro-team: '*'
  enterprise-server: '>=2.22'
---

{% data reusables.actions.enterprise-beta %}
{% data reusables.actions.enterprise-github-hosted-runners %}

{% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.22" %} Predeterminadamente, {% data variables.product.product_name %} almacena las bitácoras de compilación y los artefactos por 90 días, y puedes personalizar este periodo de retención dependiendo del tipo de repositorio. Para obtener más información, consulta la sección "[Configurar el periodo de retención para los artefactos y las bitácoras de las GitHub Actions en tu repositorio](/github/administering-a-repository/configuring-the-retention-period-for-github-actions-artifacts-and-logs-in-your-repository)".{% endif %}
{% if currentVersion == "enterprise-server@2.22" %} Las {% data variables.product.product_name %} almacenan las bitácoras y los artefactos por 90 días.{% endif %}

{% data reusables.repositories.permissions-statement-read %}

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.actions-tab %}
{% data reusables.repositories.navigate-to-workflow %}
{% data reusables.repositories.view-run %}
1. Debajo de **Artefactos**, da clic en aquél que quieras descargar.
    {% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@3.0" %}
    ![Menú desplegable Download artifact (Descargar artefacto)](/assets/images/help/repository/artifact-drop-down-updated.png)
    {% else %}
    ![Menú desplegable Download artifact (Descargar artefacto)](/assets/images/help/repository/artifact-drop-down.png)
    {% endif %}
