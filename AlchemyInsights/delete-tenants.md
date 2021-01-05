---
title: テナントの削除
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/30/2020
ms.locfileid: "49565239"
---
# <a name="delete-tenant"></a><span data-ttu-id="bb851-102">テナントの削除</span><span class="sxs-lookup"><span data-stu-id="bb851-102">Delete tenant</span></span>

<span data-ttu-id="bb851-103">Azure AD を削除するには、次のことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bb851-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="bb851-104">ディレクトリのグローバル管理者である。</span><span class="sxs-lookup"><span data-stu-id="bb851-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="bb851-105">admin@contoso.onmicrosoft.com など、contoso.onmicrosoft.com などの既定のディレクトリを持つアカウントでサインインしていない。</span><span class="sxs-lookup"><span data-stu-id="bb851-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="bb851-106">削除する前に、アクティブなアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="bb851-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="bb851-107">アクティブなアプリケーションを削除するには、[アプリの登録] に移動して既存のアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="bb851-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="bb851-108">ディレクトリに Microsoft Azure、Office 365、Azure AD Premium などの Microsoft Online Service のアクティブなサブスクリプションは関連付けられていません。</span><span class="sxs-lookup"><span data-stu-id="bb851-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="bb851-109">サブスクリプションを譲渡するか、Azure サポートと課金からアクティブなサブスクリプションのキャンセルを続行します。</span><span class="sxs-lookup"><span data-stu-id="bb851-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="bb851-110">Office 365 と Azure サブスクリプションをキャンセルする方法の詳細について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb851-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="bb851-111">テナントへの既存のサブスクリプションの関連付けや追加に関するガイダンスについては、「[Azure サブスクリプションを Azure Active Directory テナントに関連付けるまたは追加する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb851-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="bb851-112">アクティブなライセンスはありません。</span><span class="sxs-lookup"><span data-stu-id="bb851-112">There are no Active license.</span></span> <span data-ttu-id="bb851-113">ライセンスを削除するには、「[サブスクリプションを削除してライセンスを削除する方法](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb851-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="bb851-114">Azure AD を削除しようとした際、ディレクトリにはグローバル管理者であるあなた以外にアクティブなユーザーは見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="bb851-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="bb851-115">その他のアクティブなユーザーを削除します。また、admin@contoso.com で作成されたユーザーなど、テナント内のカスタム ドメイン名の依存関係も削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb851-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="bb851-116">次のことを行うための詳細なステップ:</span><span class="sxs-lookup"><span data-stu-id="bb851-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="bb851-117">"Azure Active Directory" または "サブスクリプション" を削除するには、「[Azure Active Directory を削除する](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb851-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="bb851-118">ディレクトリ内のアプリケーションを削除するには、「[アプリケーションを削除する](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb851-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
