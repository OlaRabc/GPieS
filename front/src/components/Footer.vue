<template>
    <footer class="footer">
        <h2 class="footer__title">
          Skontaktuj się z nami
        </h2>
        <div class="footer__links-section links-section">
          <div class="links-section__links">
            <p class="link">
              <a class="link__reference">
                contacty@gpies.com
              </a>
            </p>
            <p class="link">
              Nasz profil na
              <a class="link__reference">
                LinkedIn
              </a>
            </p>
          </div>
          <div class="links-section__fanpage">
            <div class="fanpage">
              <i class="fa fa-linkedin" aria-hidden="true"></i>
            </div>
            <div class="fanpage">
              <i class="fa fa-instagram" aria-hidden="true"></i>
            </div>
            <div class="fanpage">
              <i class="fa fa-youtube-play" aria-hidden="true"></i>
            </div>
            <div class="fanpage">
              <i class="fa fa-twitter" aria-hidden="true"></i>
            </div>
          </div>
        </div>
        <div class="footer__policy-section">
          <div class="policy">
            <a class="policy__link">
              Aleksandra Rabcewicz
            </a>
            <a class="policy__link">
                Filip Zytka
            </a>
            <a class="policy__link">
                Małgorzata Skowrońska
            </a>
          </div>
        </div>
      </footer>
</template>

<style scoped>
.footer {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
  background: #495f7a;
  color: #FFFFFF;
  padding: 32px;
  height: 100%;
}
.footer__title {
  margin-bottom: 40px;
}
.footer__policy-section {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
  flex-wrap: wrap;
  margin-bottom: 32px;
}

.links-section {
  margin-bottom: 56px;
}
.links-section__links {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
}
.links-section__fanpage {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  margin-right: 32px;
}

@media (min-width: 750px) {
  .links-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: row;
  }
}
.link {
  width: -webkit-max-content;
  width: -moz-max-content;
  width: max-content;
  margin-bottom: 8px;
  color: #BFBFBF;
}
.link__reference {
  text-decoration: none;
  margin-right: 32px;
  color: #FFFFFF;
}
.link__reference:hover {
  text-decoration: underline;
}

.fanpage {
  background: #FFFFFF;
  width: -webkit-min-content;
  width: -moz-min-content;
  width: min-content;
  height: -webkit-min-content;
  height: -moz-min-content;
  height: min-content;
  padding: 16px 20px;
  font-size: 20px;
  margin: 8px;
  color: #1A1A1A;
  border-radius: 50px;
  transition: background-color 0.5s, color 0.5s;
}
.fanpage:hover {
  background: #6E737A;
  color: #FFFFFF;
}

.policy {
  flex-wrap: wrap;
  margin-bottom: 8px;
}
.policy__link {
  text-decoration: none;
  color: #FFFFFF;
  transition: color 0.5s;
}
.policy__link:hover {
  color: #6E737A;
  text-decoration: underline;
}
.policy__link::after {
  content: " | ";
}
.policy__link:last-child::after {
  content: "";
}

@media (min-width: 750px) {
  .footer {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    flex-direction: column;
  }
  .footer__links-section {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    flex-direction: column;
  }
  .footer__policy-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: row;
    width: 100%;
    flex-wrap: nowrap;
  }
  .links-section__links {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    flex-direction: row;
  }
  .policy {
    margin-bottom: 0px;
  }
}
@media (min-width: 1000px) {
  .links-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: row;
    width: 100%;
  }
}
</style>