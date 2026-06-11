# SPIKES (in IVS) 2026 組織図

Notion「メンバー」ページとGoogle Sheets「組織」タブを統合。

> **凡例**: `D` = ディレクター / `P` = プランナー

```mermaid
graph TD
    Onoda["小野田 芽依<br/>D<br/>学生代表・全体統括"]

    Onoda --> CreativeHQ["クリエイティブ"]
    Onoda --> MktHQ["集客・マーケティング統括"]
    Onoda --> ContentHQ["コンテンツ統括"]
    Onoda --> PlannerHQ["プランナー"]
    Onoda --> OpsHQ["運営・管理"]

    %% 集客
    MktHQ --> Aruga["有賀 心咲<br/>D<br/>Instagram発信"]
    MktHQ --> Tatsuzaki["立崎 乃衣<br/>D<br/>データ分析"]
    MktHQ --> Ota["太田 智也<br/>東西代表マネジメント"]
    Aruga --> Tagami["田上 睦己<br/>P<br/>X発信"]
    Tatsuzaki --> Tagami
    Ota --> GUILD["GUILD"]
    Ota --> NOMAD["NOMAD"]
    GUILD --> Ozawa["小澤 剛<br/>D"]
    Ozawa --> Yamashita["山下 翼<br/>P"]
    Ozawa --> Shimakawa["島川 哲也<br/>P"]
    NOMAD --> Kishida["岸田 宗将<br/>D"]

    %% コンテンツ
    ContentHQ --> BLITZ["BLITZ"]
    ContentHQ --> STAGE["STAGE"]
    ContentHQ --> SPIKATHON["SPIKATHON"]
    ContentHQ --> SQUARE["SQUARE"]
    ContentHQ --> PITCH["PITCH"]
    BLITZ --> Kurenai["紅 優行<br/>D"]
    BLITZ --> Yamada["山田 結理奈<br/>D"]
    STAGE --> Matsuo["松尾 妃奈乃<br/>D"]
    SPIKATHON --> Kato["加藤 一路<br/>D"]
    SQUARE --> Sakamoto["坂元 柾毅<br/>D"]
    Sakamoto --> Nishikawa["西川 歩花<br/>P"]
    PITCH --> Udatsu["宇田津 蓮<br/>D"]
    Udatsu --> Saito["齋藤 杏理<br/>P"]

    %% クリエイティブ
    CreativeHQ --> Shiratori["白鳥 太智<br/>D"]

    %% プランナー
    PlannerHQ --> Azumada["東田 蒼人<br/>P"]

    %% 運営・管理
    OpsHQ --> Yoshimoto["吉本<br/>オペレーション（TBD）"]

    classDef head fill:#1f3a68,stroke:#fff,color:#fff;
    classDef group fill:#2e5aa8,stroke:#fff,color:#fff;
    classDef tbd fill:#c0392b,stroke:#fff,color:#fff;
    class Onoda head;
    class MktHQ,ContentHQ,CreativeHQ,OpsHQ,PlannerHQ group;
    class BLITZ,STAGE,SPIKATHON,SQUARE,PITCH group;
    class GUILD,NOMAD group;
    class Yoshimoto tbd;
```

## 企画コンテンツ × 担当者マップ

各コンテンツ（上段）と担当リード（下段）の対応。

```mermaid
graph TD
    subgraph マーケティング
      CP[コミュニティパートナー]
      SNS[SNS]
      EV[イベント・セミナー企画]
      INF[インフルエンサー]
      LP[LP]
      CRM[CRM]
      SNS --> Aruga2[有賀 心咲]
    end

    subgraph コンテンツ
      PITCH[PITCH]
      STAGE[SESSION / STAGE]
      SPIKATHON[SPIKATHON]
      NW[ネットワーク]
      NW --> SQUARE[SQUARE]
      NW --> BLITZ["BLITZ（ライトニング）"]
      NW --> ROUND["ROUND（テーブル）"]
      NW --> MARKET["Market（ブース）"]
      POPUP[POPUP]
      GUILD[GUILD]

      PITCH --> Udatsu2[宇田津 蓮]
      STAGE --> Matsuo2[松尾 妃奈乃]
      SPIKATHON --> Kato2[加藤 一路]
      SQUARE --> Sakamoto2[坂元 柾毅]
      BLITZ --> Kurenai2[紅 優行]
      BLITZ --> Yamada2[山田 結理奈]
      POPUP --> Ozawa2[小澤 剛]
      GUILD --> Ozawa2
    end

    subgraph 人事組織
      RECRUIT[採用]
      GROW[管理・育成]
    end

    classDef role fill:#2e5aa8,stroke:#fff,color:#fff;
    classDef person fill:#f2b84b,stroke:#333,color:#111;
    class CP,SNS,EV,INF,LP,CRM,PITCH,STAGE,SPIKATHON,NW,SQUARE,BLITZ,ROUND,MARKET,POPUP,GUILD,RECRUIT,GROW role;
    class Aruga2,Udatsu2,Matsuo2,Kato2,Sakamoto2,Ozawa2,Kurenai2,Yamada2 person;
```

## 元データ
- Notion: https://www.notion.so/techweek/34257f3cbb7880e5a7c9fdb76ac4ffc4
- Google Sheets: https://docs.google.com/spreadsheets/d/1K-MvzzDbFs6m05ytU3WtkOfGm3vV99TrSTWF5ajYbSU
