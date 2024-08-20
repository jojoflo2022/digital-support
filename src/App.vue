<template>
  <!-- ローディングアニメーションコンテナ -->
  <div id="loading" class="loading-container" v-show="isLoading">
    <!-- テニスボールの画像 -->
    <img
      src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digisuisin_01.png"
      alt="Loading..."
      class="tennis-ball"
    />
  </div>

  <header v-show="!isLoading">
    <nav>
      <ul class="nav-list">
        <li>
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/05/Instagram01.html"
            target="_blank"
            >Instagramの登録方法</a
          >
        </li>
        <li>
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/howto03.html"
            target="_blank"
            >Instagramの使い方</a
          >
        </li>
        <li>
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/05/snspre01.html"
            target="_blank"
            >SNSの注意点</a
          >
        </li>
        <li>
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/05/smaho01.html"
            target="_blank"
            >スマートフォン活用ガイド</a
          >
        </li>
        <li>
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/08/prt.html"
            target="_blank"
            >スマホでのプリント方法</a
          >
        </li>
        <li>
          <a href="https://lin.ee/DP0aI2A" target="_blank"
            ><img
              class="line"
              src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/line_01.png"
              alt="LINEロゴ"
          /></a>
          <a
            href="https://www.instagram.com/minamifurano_town/
          "
            target="_blank"
            ><img
              class="inst"
              src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/instagram_01.png"
              alt="Instagramロゴ"
          /></a>
        </li>
      </ul>
    </nav>
    <div class="hamburger" @click="toggleMenu">
      <span class="bar"></span>
      <span class="bar"></span>
      <span class="bar"></span>
    </div>
  </header>

  <main v-show="!isLoading">
    <section class="hero-container">
      <div class="hero">
        <div class="hero-image" id="heroImage1"></div>
        <div class="hero-image" id="heroImage2"></div>
      </div>
      <div class="hero-text">
        <p>地域コミュニティの強化</p>
        <h1>デジタル推進委員<br />サポートルーム</h1>
      </div>
    </section>

    <section class="hero-container-2">
      <div class="hc2 animated-element">
        <h2>サポートルームの目的</h2>
        <p>
          サポートルームは、LINEやInstagramを使って地域の情報共有を促進し、
          町民がデジタル技術に親しむ場を提供します。<br />初心者から経験者まで、
          どなたでも気軽に参加でき、デジタル世界での地域連携を強化します。
        </p>
        <h2>参加のご案内</h2>
        <p>
          サポートルームへの参加は無料で、開催日は調整中です。当日会場にお越しください。
        </p>
      </div>

      <div class="hc2_wrapper animated-element">
        <h2>サポート内容</h2>
        <p>サポートします</p>
        <p>日常生活でSNSを効果的に使えるよう</p>
        <p>スマホの使い方など</p>
        <p>デジタル全般の疑問や悩みにも対応し</p>
        <p>実践的な活用方法を学べる講座を提供</p>
        <p>SNSの基本操作やアカウント設定</p>
        <p>サポートルームでは</p>
      </div>
    </section>

    <div class="products-text animated-element">
      <h2>サポートリンク</h2>
    </div>

    <section class="products">
      <div class="product-container animated-element">
        <h3>Instagramの登録方法</h3>
        <div
          class="product-card"
          style="
            background-image: url('https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_01.jpg');
          "
        >
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/05/Instagram01.html"
            target="_blank"
          >
          </a>
        </div>
      </div>
      <div class="product-container animated-element">
        <h3>Instagramの使い方</h3>
        <div
          class="product-card"
          style="
            background-image: url('https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_02.jpg');
          "
        >
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/howto03.html"
            target="_blank"
          >
          </a>
        </div>
      </div>
      <div class="product-container animated-element">
        <h3>SNSの注意点</h3>
        <div
          class="product-card"
          style="
            background-image: url('https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_04.jpg');
          "
        >
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/05/snspre01.html"
            target="_blank"
          >
          </a>
        </div>
      </div>
      <div class="product-container animated-element">
        <h3>スマホ活用ガイド</h3>
        <div
          class="product-card"
          style="
            background-image: url('https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/08/prt_01.jpg');
          "
        >
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/05/smaho01.html"
            target="_blank"
          >
          </a>
        </div>
      </div>
      <div class="product-container animated-element">
        <h3>スマホでのプリント方法</h3>
        <div
          class="product-card"
          style="
            background-image: url('https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_03.jpg');
          "
        >
          <a
            href="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/08/prt.html"
            target="_blank"
          >
          </a>
        </div>
      </div>
    </section>

    <section class="eigyou animated-element">
      <div class="e-product-container">
        <div class="e-product-card animated-element"></div>
      </div>
    </section>

    <section class="ryoukin">
      <div class="r-products-text animated-element">
        <h2>よくある質問</h2>
        <div class="price-table-container">
          <div class="price-table-wrapper">
            <table class="price-table animated-element">
              <tr>
                <th colspan="2">
                  Q: SNSとは何ですか？どのようなメリットがありますか？
                </th>
              </tr>
              <tr class="highlight">
                <td class="label">
                  A:
                  SNS（ソーシャルネットワーキングサービス）は、オンライン上で人々が交流し、
                  情報を共有するためのプラットフォームです。友達や家族とのコミュニケーション、
                  趣味や興味を共有できる場の提供、地域イベントの情報収集など、
                  日常生活に役立つ様々なメリットがあります。
                </td>
              </tr>
            </table>
          </div>
          <div class="price-table-wrapper">
            <table class="price-table animated-element">
              <tr>
                <th colspan="2">
                  Q:
                  デジタル推進委員サポートルームではどのようなサポートを受けられますか？
                </th>
              </tr>
              <tr class="highlight">
                <td class="label">
                  A:
                  LINEやInstagramなどの主要なSNSの基本操作から応用的な使い方まで、
                  幅広くサポートいたします。アカウントの設定方法、メッセージの送受信、
                  写真や動画の投稿方法など、実践的なスキルを身につけていただけます。
                </td>
              </tr>
            </table>
          </div>
          <div class="price-table-wrapper">
            <table class="price-table animated-element">
              <tr>
                <th colspan="2">
                  Q: SNSを安全に利用するために気をつけるべきことは何ですか？
                </th>
              </tr>
              <tr class="highlight">
                <td class="label">
                  A:
                  パスワードを定期的に変更し、個人情報の公開は最小限に留めることが重要です。
                  見知らぬ人からのメッセージやリンクには注意し、不審な場合は開かないようにしましょう。
                  また、プライバシー設定を適切に管理し、
                  自分の投稿が意図しない相手に見られないよう配慮することも大切です。
                </td>
              </tr>
            </table>
          </div>
          <div class="price-table-wrapper">
            <table class="price-table animated-element">
              <tr>
                <th colspan="2">
                  Q: SNSで写真や動画を共有する際の注意点を教えてください。
                </th>
              </tr>
              <tr class="highlight">
                <td class="label">
                  A: 写真や動画を投稿する際は、個人情報が含まれていないか、
                  公開しても問題ない内容かを十分に確認しましょう。他者のプライバシーにも配慮し、
                  許可なく撮影・投稿することは避けてください。SNSは多くの人が閲覧する場であることを意識し、
                  適切な内容の投稿を心がけることが大切です。
                </td>
              </tr>
            </table>
          </div>
          <div class="price-table-wrapper">
            <table class="price-table animated-element">
              <tr>
                <th colspan="2">
                  Q: SNSでの友達づくりのコツを教えてください。
                </th>
              </tr>
              <tr class="highlight">
                <td class="label">
                  A:
                  友達や知人の名前で検索したり、共通の友達を介して新しい人脈を見つけることができます。
                  コミュニティやグループに参加することで、同じ興味を持つ人々と交流するのも効果的です。
                  ただし、見知らぬ人からの友達リクエストは慎重に判断し、
                  必要に応じて拒否するようにしましょう。安全性を確保しながら、
                  SNSを通じて有意義な人間関係を築いていくことが大切です。
                </td>
              </tr>
            </table>
          </div>
        </div>
      </div>
    </section>

    <section class="visuals-icon animated-element">
      <a href="https://lin.ee/DP0aI2A" target="_blank"
        ><img
          class="line"
          src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/line_01.png"
          alt="LINEロゴ"
      /></a>
      <a
        href="https://www.instagram.com/minamifurano_town/
        "
        target="_blank"
        ><img
          class="inst"
          src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/instagram_01.png"
          alt="Instagramロゴ"
      /></a>
    </section>

    <section class="profile-section animated-element">
      <div class="profile-content">
        <div class="profile-images">
          <img
            src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/IMG_E2109.jpg"
            alt="中谷仁彦の写真"
            class="personal-image"
          />
          <img
            src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/04/image_20240423182100.png"
            alt="デジタル推進委員の画像"
            class="committee-image"
          />
        </div>
        <div class="profile-description">
          <h2>プロフィール</h2>
          <p>
            中谷 仁彦<br />(なかや よしひこ)<br />
            1977/10/16生まれ<br />
            南富良野町地域おこし協力隊<br />南富良野町をもっとたくさんの人に知ってもらうために、<br />
            町民みんなが<br />「#ナンプルエンサー」となり、<br />
            町の魅力をどんどん発信していける環境を作る場にできたらと考えています。
          </p>
          <p>
            Instagram:
            <a href="https://www.instagram.com/nanpu_nakaya/" target="_blank"
              >@nanpu_nakaya</a
            >
          </p>
        </div>
      </div>
    </section>

    <div class="m-product-container">
      <div class="m-product-card animated-element"></div>
    </div>
  </main>

  <footer>
    <div class="sdgs-logos">
      <img
        src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/sdg_icon_04_ja_2.png"
        alt="SDGs Goal 4"
      />
      <img
        src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/sdg_icon_09_ja_2.png"
        alt="SDGs Goal 9"
      />
      <img
        src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/sdg_icon_11_ja_2.png"
        alt="SDGs Goal 11"
      />
      <img
        src="https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/01/sdg_icon_17_ja_2.png"
        alt="SDGs Goal 17"
      />
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      isLoading: true,
      currentImageIndex: 0,
      currentDiv: 1,
      images: [
        "https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_01.jpg",
        "https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_05.jpg",
        "https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_02.jpg",
        "https://www.town.minamifurano.hokkaido.jp/wp-content/uploads/2024/06/digi_04.jpg",
      ],
    };
  },
  mounted() {
    // ローディングアニメーションの表示
    this.showLoading();
  },
  methods: {
    showLoading() {
      setTimeout(() => {
        this.isLoading = false;
        this.setInitialImage();
        this.startImageRotation();
        window.addEventListener("scroll", this.checkAnimation);
      }, 1200);
    },
    toggleMenu() {
      const hamburger = document.querySelector(".hamburger");
      const navList = document.querySelector(".nav-list");
      hamburger.classList.toggle("active");
      navList.classList.toggle("show");
    },
    changeImage() {
      this.currentImageIndex =
        (this.currentImageIndex + 1) % this.images.length;
      this.currentDiv = 3 - this.currentDiv;
      const currentHeroImage = document.getElementById(
        `heroImage${this.currentDiv}`
      );
      const otherHeroImage = document.getElementById(
        `heroImage${3 - this.currentDiv}`
      );

      currentHeroImage.style.backgroundImage = `url("${
        this.images[this.currentImageIndex]
      }")`;
      currentHeroImage.classList.add("zoom-out", "show");

      setTimeout(() => {
        currentHeroImage.classList.remove("zoom-out");
      }, 1500);

      otherHeroImage.classList.remove("show");
    },
    setInitialImage() {
      const heroImage1 = document.getElementById("heroImage1");
      heroImage1.style.backgroundImage = `url("${this.images[0]}")`;
      heroImage1.classList.add("show");
    },
    startImageRotation() {
      setInterval(this.changeImage, 5000);
    },
    checkAnimation() {
      const animatedElements = document.querySelectorAll(".animated-element");
      animatedElements.forEach((element) => {
        const elementTop = element.getBoundingClientRect().top;
        const elementBottom = element.getBoundingClientRect().bottom;
        const windowHeight = window.innerHeight;

        if (elementTop < windowHeight && elementBottom > 0) {
          element.classList.add("faded-bounce");
        } else {
          element.classList.remove("faded-bounce");
        }
      });
    },
  },
  beforeUnmount() {
    // スクロールイベントの監視を停止
    window.removeEventListener("scroll", this.checkAnimation);
  },
};
</script>

<style></style>
