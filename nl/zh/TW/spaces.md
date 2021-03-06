---

copyright:

  years: 2018
lastupdated: "2018-04-13"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}

# 決定空間
{: #determinespaces}

在組織內，空間提供額外層次的界限強制執行及抽象化。

空間是組織中的保留區域，使用者可以在其中開發及執行應用程式和服務。您可以在組織中建立任意數量的空間，也可以控制有權存取空間的使用者。如需詳細資料，請參閱[空間](/docs/account/orgs_spaces.html#orgsspacesusers)。

如果您計劃定義許多空間，則可以建立應用程式來協助管理空間。當空間數超過 60 個時，建議您考慮再定義另一個組織。

## 單一組織與多組織的空間
{: #spaceconsiderations}

當您採用單一組織架構時，會依照您在組織內定義的空間來提供隔離和抽象化層次。在定義空間時，請考量下列指引：

* 定義一個用來管理服務的空間，只需要在組織中佈建及配置一次。
* 根據交付生命週期來定義空間。例如，您可以為正在開發的應用程式定義一個以上的空間、為處於測試階段的應用程式定義一個以上的空間，以及為處於正式作業的應用程式定義一個以上的空間。
* 如果交付生命週期界限不足，您可以為每個 LOB 和交付階段各定義一個以上的空間，以加強隔離。
* 識別您是否需要為不同的使用者群組強制執行界限。例如，開發人員無法開發應用程式並進行測試。您需要一組不同的使用者來測試應用程式。在此情境中，您會建立兩個空間，一個供應用程式的開發人員使用，一個供應用程式的測試人員使用。然後，將正確空間的存取權授與給各組使用者。

當您實作多組織架構時，可以依 LOB 及/或交付生命週期來將各組織隔離。然後，您可以根據公司內相同部門交付的應用程式或專案數目來定義多個空間。在計劃組織中的空間時，請考量下列指引：

* 定義一個用來管理服務的空間，只需要在組織中佈建及配置一次。
* 為每個應用程式、相關應用程式的每個群組，或為特定專案定義空間。
* 如果您需要為不同的使用者強制執行界限，請為每一組使用者定義一個空間。當使用者被授與空間中的開發人員角色時，該使用者即具有完整的存取權，可以存取在該空間中佈建及執行的任何資源和 {{site.data.keyword.Bluemix_notm}} 服務。如果您需要強制執行更嚴密的安全措施，以防止使用者控制每項資源，請考慮定義不同的空間。在所有這些空間內，您都可以佈建 {{site.data.keyword.Bluemix_notm}} 服務，以供該空間中執行的應用程式使用。

## 空間命名、限制及管理
{: #spaceadmin}

若要為雲端組織定義不同的空間，請考量下列指引：

* 定義並強制執行命名慣例。例如，定義一個命名慣例，讓空間名稱包含組織所在位置以及雲端類型的相關資訊。您可以在建立空間之後變更它的名稱。如果空間名稱有所變更，請通知所有空間團隊成員有關變更的資訊。
* 定義適用於空間的限制。例如，定義可在每個空間中開發、管理及部署的應用程式類型。
* 識別空間的管理員。建議您將空間管理工作委派給多個人員。
