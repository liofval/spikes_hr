# SPIKES (in IVS) 2026 組織図

Notion「メンバー」ページとGoogle Sheets「組織」タブを統合。

> **凡例**: `D` = ディレクター / `P` = プランナー

## ロール階層

```mermaid
%%{init: {'flowchart': {'nodeSpacing': 20, 'rankSpacing': 25}, 'themeVariables': {'fontSize': '11px'}}}%%
graph TD
    R["代表<br/>小野田・小澤・岸田"]
    D["ディレクター<br/>有賀・立崎・紅・山田・松尾<br/>加藤・坂元・宇田津・白鳥・井上"]
    P["プランナー<br/>田上・西川・齋藤・東田<br/>山下・島川・宇治・川合・村瀬・吉岡"]
    A["アシスタント（当日企画補佐）<br/>（TBD）"]
    C["クルー（当日会場補佐）<br/>（TBD）"]
    R --> D --> P --> A --> C

    classDef role fill:#2e5aa8,stroke:#fff,color:#fff;
    class R,D,P,A,C role;
```

## 組織図

```mermaid
graph TD
    Onoda["小野田 芽依<br/>D<br/>学生代表・全体統括"]

    Onoda --> MktHQ["マーケ・クリエイティブ"]
    Onoda --> PromoHQ["集客"]
    Onoda --> ContentHQ["コンテンツ統括"]
    Onoda --> OpsHQ["運営・管理"]

    %% マーケ・クリエイティブ
    MktHQ --> Aruga["有賀 心咲<br/>D<br/>Instagram発信"]
    MktHQ --> Tatsuzaki["立崎 乃衣<br/>D<br/>データ分析"]
    MktHQ --> Shiratori["白鳥 太智<br/>D<br/>クリエイティブ"]
    MktHQ --> Inoue["井上 颯<br/>D<br/>クリエイティブ"]
    Aruga --> Tagami["田上 睦己<br/>P<br/>X発信"]
    Tatsuzaki --> Tagami

    %% 集客
    PromoHQ --> GUILD["GUILD"]
    PromoHQ --> NOMAD["NOMAD"]
    GUILD --> Ozawa["小澤 剛<br/>D"]
    Ozawa --> Yamashita["山下 翼<br/>P"]
    Ozawa --> Shimakawa["島川 哲也<br/>P"]
    NOMAD --> Kishida["岸田 宗将<br/>D"]
    Kishida --> Azumada["東田 蒼人<br/>P"]

    %% コンテンツ
    ContentHQ --> BLITZ["BLITZ"]
    ContentHQ --> STAGE["STAGE"]
    ContentHQ --> SPIKATHON["SPIKATHON"]
    ContentHQ --> SQUARE["SQUARE"]
    ContentHQ --> PITCH["PITCH"]
    BLITZ --> Kurenai["紅 優行<br/>D"]
    BLITZ --> Yamada["山田 結理奈<br/>D"]
    Kurenai --> Uji["宇治 大輝<br/>P"]
    Yamada --> Kawai["川合 正宗<br/>P"]
    STAGE --> Matsuo["松尾 妃奈乃<br/>D"]
    Matsuo --> Yoshioka["吉岡 夏輝<br/>P"]
    SPIKATHON --> Kato["加藤 一路<br/>D"]
    Kato --> Murase["村瀬 智哉<br/>P"]
    SQUARE --> Sakamoto["坂元 柾毅<br/>D"]
    Sakamoto --> Nishikawa["西川 歩花<br/>P"]
    PITCH --> Udatsu["宇田津 蓮<br/>D"]
    Udatsu --> Saito["齋藤 杏理<br/>P"]

    %% 運営・管理
    OpsHQ --> Ota["太田 智也<br/>東西代表マネジメント"]
    OpsHQ --> Yoshimoto["吉本<br/>オペレーション（TBD）"]
    Ota --> Onoda
    Yoshimoto --> Onoda

    classDef head fill:#1f3a68,stroke:#fff,color:#fff;
    classDef group fill:#2e5aa8,stroke:#fff,color:#fff;
    classDef tbd fill:#c0392b,stroke:#fff,color:#fff;
    class Onoda head;
    class MktHQ,PromoHQ,ContentHQ,OpsHQ group;
    class BLITZ,STAGE,SPIKATHON,SQUARE,PITCH group;
    class GUILD,NOMAD group;
    class Yoshimoto,Ota tbd;
```

## 企画コンテンツ × 担当者マップ

各コンテンツ（上段）と担当リード（下段）の対応。

```mermaid
graph TD
    subgraph SG_MC ["マーケ・クリエイティブ"]
      SNS[SNS]
      DATA[データ分析]
      EV[イベント・セミナー企画]
      LP[LP]
      CREATIVE[クリエイティブ全般]
      SNS --> Aruga2[有賀 心咲<br/>Instagram]
      SNS --> Tagami2[田上 睦己<br/>X]
      DATA --> Tatsuzaki2[立崎 乃衣]
      LP --> Onoda3[小野田 芽依]
      CREATIVE --> Shiratori2[白鳥 太智]
      CREATIVE --> Inoue2[井上 颯]
      CREATIVE --> Shimakawa3[島川 哲也]
    end

    subgraph SG_PROMO ["集客"]
      GUILD[GUILD]
      NOMAD[NOMAD]
      GUILD --> POPUP[POPUP]
      GUILD --> Ozawa2[小澤 剛]
      Ozawa2 --> Yamashita2[山下 翼]
      Ozawa2 --> Shimakawa2[島川 哲也]
      NOMAD --> Kishida2[岸田 宗将]
      HAIBATSU[派閥]
      HAIBATSU --> ArugaP[有賀 心咲]
      HAIBATSU --> KatoP[加藤 一路]
      ArugaP --> PALL["P<br/>田上・西川・齋藤・東田<br/>山下・島川・宇治・川合・村瀬"]
      KatoP --> PALL
    end

    subgraph SG_CONT ["コンテンツ"]
      PITCH[PITCH]
      STAGE[STAGE]
      SPIKATHON[SPIKATHON]
      SQUARE[SQUARE]
      BLITZ[BLITZ]
      NW[ネットワーク]
      NW --> ROUND["ROUND（テーブル）"]
      NW --> MARKET["Market（ブース）"]

      PITCH --> Udatsu2[宇田津 蓮]
      Udatsu2 --> Saito2[齋藤 杏理]
      STAGE --> Matsuo2[松尾 妃奈乃]
      Matsuo2 --> Yoshioka2[吉岡 夏輝]
      SPIKATHON --> Kato2[加藤 一路]
      Kato2 --> Murase2[村瀬 智哉]
      SQUARE --> Sakamoto2[坂元 柾毅]
      Sakamoto2 --> Nishikawa2[西川 歩花]
      BLITZ --> Kurenai2[紅 優行]
      BLITZ --> Yamada2[山田 結理奈]
      Kurenai2 --> Uji2[宇治 大輝]
      Yamada2 --> Kawai2[川合 正宗]
    end

    subgraph SG_HR ["人事組織"]
      RECRUIT[採用]
      RECRUIT --> Onoda2[小野田 芽依]
      Onoda2 --> Matsuo3[松尾 妃奈乃]
      Onoda2 --> Kurenai3[紅 優行]
    end

    classDef role fill:#2e5aa8,stroke:#fff,color:#fff;
    classDef person fill:#f2b84b,stroke:#333,color:#111;
    class SNS,DATA,EV,LP,GUILD,NOMAD,CREATIVE,PITCH,STAGE,SPIKATHON,NW,SQUARE,BLITZ,ROUND,MARKET,POPUP,RECRUIT,HAIBATSU,PALL role;
    class Aruga2,Tagami2,Tatsuzaki2,Ozawa2,Yamashita2,Shimakawa2,Shimakawa3,Kishida2,Shiratori2,Inoue2,Udatsu2,Saito2,Matsuo2,Matsuo3,Kato2,Sakamoto2,Nishikawa2,Kurenai2,Kurenai3,Yamada2,Onoda2,Onoda3,Uji2,Kawai2,Murase2,ArugaP,KatoP,Yoshioka2 person;
```

## 元データ
- Notion: https://www.notion.so/techweek/34257f3cbb7880e5a7c9fdb76ac4ffc4
- Google Sheets: https://docs.google.com/spreadsheets/d/1K-MvzzDbFs6m05ytU3WtkOfGm3vV99TrSTWF5ajYbSU
