---
title: パスワード同期
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484083"
---
# <a name="password-synchronization"></a><span data-ttu-id="ebf71-102">パスワード同期</span><span class="sxs-lookup"><span data-stu-id="ebf71-102">Password synchronization</span></span>

<span data-ttu-id="ebf71-103">[**パスワード ハッシュ同期がまったく動作しない**]</span><span class="sxs-lookup"><span data-stu-id="ebf71-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="ebf71-104">パスワード ハッシュ同期が機能しない場合にお客様が遭遇する一般的な問題は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ebf71-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="ebf71-105">オンプレミスの Active Directory と通信するために Azure AD Connect によって使用される Active Directory アカウントには、**ディレクトリ変更の複製** と **ディレクトリ変更の複製パスワード同期** に必要なすべてのアクセス許可が付与されていません。これらのアクセス許可を Active Directory アカウントに付与して、これを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebf71-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="ebf71-106">管理者がユーザーサインイン方法を **パスワード同期** から Azure AD Connect ウィザードの **AD FS とのフェデレーション** などの別のオプションに変更した後、パスワード ハッシュ同期は無効になります。Azure AD Connect ウィザードで **パスワード ハッシュ同期** 機能を再度有効にすることで、これを修正できます。</span><span class="sxs-lookup"><span data-stu-id="ebf71-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="ebf71-107">オンプレミスの Active Directory での接続の問題。</span><span class="sxs-lookup"><span data-stu-id="ebf71-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="ebf71-108">たとえば、一部のドメインコントローラーに Azure AD Connect からアクセスできない場合や、[必要なポート](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)がファイアウォールによってブロックされている場合などがあります。Azure AD Connect サーバーとオンプレミスの Active Directory の間の接続が正しく機能することを確認して、これを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebf71-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="ebf71-109">Azure AD Connect サーバーは現在ステージング モードになっているため、サーバーはパスワード ハッシュを実行できません。問題のトラブルシューティングを行うには、「[Azure AD Connect 同期を使用したパスワード同期のトラブルシューティング - パスワードが同期されません](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)」セクションで説明されている手順に従います。</span><span class="sxs-lookup"><span data-stu-id="ebf71-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="ebf71-110">[**一部のユーザーでパスワード ハッシュ同期が機能しない**]</span><span class="sxs-lookup"><span data-stu-id="ebf71-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="ebf71-111">パスワード ハッシュがユーザーに対して同期されていないことに気付いた場合は、Azure AD Connect の **トラブルシューティング** タスクを使用して、問題を調査し、解決してください。</span><span class="sxs-lookup"><span data-stu-id="ebf71-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="ebf71-112">次のタスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="ebf71-112">Perform the following tasks:</span></span>

    <span data-ttu-id="ebf71-113">a.</span><span class="sxs-lookup"><span data-stu-id="ebf71-113">a.</span></span> [<span data-ttu-id="ebf71-114">ウィザードでトラブルシューティング タスクを実行する</span><span class="sxs-lookup"><span data-stu-id="ebf71-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="ebf71-115">b.</span><span class="sxs-lookup"><span data-stu-id="ebf71-115">b.</span></span> [<span data-ttu-id="ebf71-116">トラブルシューティング コマンドレットを使用して、特定の用途のパスワード ハッシュ同期の問題を調査します</span><span class="sxs-lookup"><span data-stu-id="ebf71-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="ebf71-117">オンプレミスの Active Directory ユーザー オブジェクトで **ユーザーは次回のログオン時にパスワード変更が必要** オプションが有効になっています。</span><span class="sxs-lookup"><span data-stu-id="ebf71-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="ebf71-118">このオプションを有効にすると、ユーザーに一時パスワードが割り当てられ、次回のログオン時にパスワードを変更するように求められます。</span><span class="sxs-lookup"><span data-stu-id="ebf71-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="ebf71-119">Azure AD Connect は、一時パスワードを Azure AD に同期しません。</span><span class="sxs-lookup"><span data-stu-id="ebf71-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="ebf71-120">上記の問題を解決するには、次のいずれかのタスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="ebf71-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="ebf71-121">オンプレミス アプリケーション (Windows デスクトップなど) にサインインしてパスワードを変更するようにユーザーに依頼します。</span><span class="sxs-lookup"><span data-stu-id="ebf71-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="ebf71-122">新しいパスワードは Azure AD に同期されます。</span><span class="sxs-lookup"><span data-stu-id="ebf71-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="ebf71-123">**[ユーザーは次回のログオン時にパスワード変更が必要]** オプションを有効にせずに、管理者にユーザーのパスワードを更新してもらい、新しいパスワードをユーザーと共有します。</span><span class="sxs-lookup"><span data-stu-id="ebf71-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="ebf71-124">オンプレミスの Active Directory ユーザー オブジェクトが、オブジェクトの同期またはパスワードの同期用に **正しく構成されていません**。</span><span class="sxs-lookup"><span data-stu-id="ebf71-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="ebf71-125">この問題のトラブル シューティングを行うには、「[Azure AD Connect Sync を使用したパスワード ハッシュ同期のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)」で説明されている手順に従います。</span><span class="sxs-lookup"><span data-stu-id="ebf71-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







