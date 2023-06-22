<!-- eslint-disable vue/multi-word-component-names -->
<script setup>
import header from "../../data/Header";
</script>

<template>
  <div class="header pt-3">
    <div class="container px-lg-5 px-3">
      <div class="d-md-flex d-none justify-content-between mb-3">
        <div class="d-flex">
          <AtomSubtitle class="font-primary me-4" text="Personal" />
          <AtomSubtitle class="font-primary me-4" text="Business" />
          <AtomSubtitle class="font-primary me-4" text="About Indosat Ooredoo" />
          <AtomSubtitle class="font-primary me-4" text="Investor Relations" />
        </div>
        <div class="d-flex">
          <AtomSubtitle class="font-primary me-4" text="English" />
          <AtomSubtitle class="font-dark" text="Bahasa Indonesia" />
        </div>
      </div>
      <div class="card card-indosat mb-4">
        <div class="card-body p-0">
          <nav class="navbar navbar-expand-lg bg-transparent py-0 px-md-5 px-0">
            <div class="container">
              <a class="navbar-brand me-4" href="#"
                ><img
                  src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAQIAAADDCAMAAABeUu/HAAAAz1BMVEX///8iHiDtHCQAAADsAAAQCQ2NjIwVDxIcFhl4dne+vb7w8PCenZ4MAAgYExbm5eVkYmOrqqvtFR7sABJeXF3tEhzsAArtCxdta2zzgYT0j5L+8/P71NXzfH//+vrxZWn2qav83d760NH96+v1mZv2o6XxX2PvQEXtICjybnHydHf85OX60dL5x8j4v8D0jpDuNjzuKTD3srTvSU7vP0TQ0NAoJCZVU1TwV1z5wsPuMTf3r7DHx8ednJySkZGoqKg5NjdIRUczLzF/fn5NSkweMw+cAAARU0lEQVR4nO1daXuqOhBWiNUu2lMoULXuu5661NrNrqf3//+mC4QlyySg1vpoeT/ceyqQmbyZzEwmEVOpBAkSJEiQIEGCBAnEuO5Miu2n6q7V2B3qCjJ1XUeo+EtJKPeQpmDo5vWutdkFyn1LCaCh5q712QHmBAM2UHnXCv04lohiQLG6u9box9HXaAoUNNq1Sj+MBmMEtkts71qnH0bdZCkwfttMKOksBdp01zr9MCY8Bc+71umH0eEnwuOudfphNHl3ONm1Tj8NzgrQr8uR2wwH2t2uNfp5KHRuhBq7Vujn0UAkB6iza312gYYeBEYD1XetzW5QHSLTMjRDR/NfOAs8lOvD+bzW/r0EJEiQIEGCBAlCnL5cXJycr/zY+cvF65GNV/vh0xWkLU7e3+zH3s5OFrEfW1zExAptEq1fqi7+Xazw0MvRp/NMPmMj7/zr/uo9Bokvbw/BY+5zmT9nsbh/VeMjfxmvzQBfaiHtIqf+i/nkyR9b91yaRkFVc18L6WOX0GN5NX0ULfcsn44Pu81/Z/GN4VINH82pMTg4Pcr7pHHIqPdngr3ZxbEqeezz5DspcLqSV79ikvClUg9mojaXT7/UjFR2Xj0CRC/+U7NSjdW0fBquSkHaIfY1DgMLlXnsSn7/WwQBWPQb89T5g8raP0DCv5fvpSCdjjWzH1jblE6FRVoFRbHI56jeHAlnAIWceiW2wbUosJt8j2LglOtSXmI8X/EIcKCG1rS4j619Ni80hPUosBX5iqDghOtU7kFI10d8BuzZkPbM6Sx6DpAaH30zBWn1j5yCN2BmC25dxLPmADnV9W9/VuHN0VgwBGtTEMXBEU9BDr6Tt5do2cep8/to78kg8wE6hPUpiJgLsSlYgwHbr3xyiVAMFO6heL4BBWlVFm/jUrAWA3Zbaz1VuAfsYBMKpGEuJgVs9rBlFD6+mYIc0OBqFJz/LAO2P7j8XgrSkvQgHgX/1jPoTVRm88sNKUirm1FwtbJX3xwqu+TckII8x+kqFKzpCjcEq8aGFIjNIA4FG8peE5ljWovYJRNBHBYGxhgUfImnQcERmXP+m18pc8w4mqbdmpH4JmYqnJ6fxsH54vUfaLW5z7UpEEcDVf1zget0p4v3BzWusWTV+yOvTnl+8pUWpt1CnSPxkoZKE6qggBJNwR+Biuo9bVmnZ4U4PqOgXtGju7gULaNUWflAjktgPEQzIZICgREUoEAbY02oXvJ52uITlrG+Gdgc8HaQFRSDIik4Bstd+U/Qqk4/I2aDYCTeYA64wLgCoPbWo4Avqbi6CatrV7LJkMuKUvUX8DHRuMUBEMkFziCKggtIN/UYbMvFsZiDXFZc0YUXIeoGXxS651uDjSqKgv+A2V0Q1pUcALPQV0FWlQTtQI2qrEvAF4MErUVQAM6DvHxsePpj9ecIEFWIqHnJwHMqcEQRFEC5cdTQCBbW2ajuQGsx8eImEnwoW4+CL96qZUtvDDiTEGUmAaCpsEFMACiAF8wRFHzwIxM9P8FUIhtVy4aFRe4CCMEb43pWAHQmHy0d8qExNiuB6BODuPitreUOgfHMSgKipC/pf9GPAb53gwTxkpuOawVFYHrGiVMAcxnRDgmJT956svH6ywPgU2CIcgqgFCvOCYT1mIOc79oh4Sp2W3IK3vmUP9KxO+AdWyzXvq44AMDgiXYK5RQAxapYwwLMwzjGEz+vjwIUYDOC/eLtUMBnBj9LwSuYbQsM8QApqJ7AlbOC4P69peDl7djBFYcPFS7cCGPSnlLwqqqZrIMCB1HhSqjBXlKw2lkPjAK/RbfPFNxLz67BEEflfaTgzxr7e5Kl+h5SsNZGvySy7CEFV6sdecLNSBbde0jBGkaQlVU794+CdY57FGTVzl9BgXyZ+isokBde9o+CdXyB9ODhHlIg2uqWciDZpN5DCuD9xwhICnB7SEHqYY38OC+uXe4jBaeFdaaCMD3cRwpSp/erzwVx8X8vKXD2YFWgVCArF4jNYE8pSFUvvi5BPKQF577yZwdGgQSn7zmIhJxoP+sAKUjBZxWEKhwmBeC5iLxgwXygFEA7u6IjK4dKAZRGCzLEg6UAWFCudehujyngv4a73vmCfabg/XtOmewzBd901mifKfimQ3cJBXtNwTedPt1nCr7pDPI+U8Cf5/1tQRE6L/jLUqN7vnaSge88VAqAL9iKDlkcKAXQ94NEZaODpGDxAR3C+DUlk9Pzi//AI2cHUDiL/5o3uIgsfFnR/lCw8TfX97+IviEFh7CVsulbLA5gQ20zCg5iW3UzCkRnsH8PBYdxxGKjt1vJvhn1KyjISL9kvR0K+AOisbK8LVGQ/ZBK3Q4FfKuC1+f9BAURDGyJAq4v8b51uhUK8lHf9twOBVW2L7FcwVYokL1uYpsUsC8nycf4lu9WKMhK33S4VQpSn2S7UbNxWxTk1MsYXnhbFKT+C7ujxv3u9fdSUFA/Y739YGsUpN4zaiaXy2XVeK+k/mYKCir7CikxBWqWQYZ4QcErdzW7wveoX44ePj6PV3jb/gkgLqSAvwjDed9+/uokdrnp4pgHodMVd3GDVw1FYgGIC3pycvwVAtDax9fR+8vqv/SQIEGCBAkSJEiQQIRyWX69Wo54E2PkDbuXIH5wXOmZyIbxWLqBbhjVB8/OdTSrdcCfIW22u4pz3byr3EJaVMfFue7cYM0noITWcjh1JfQFP3R63e723Rumw2ULuuFpMrec6/q8OF71rZk3XVsz7xeHDVvP4oi5oT5FpneDZplo1mEktCY60o3whvmYaeBvjZYwZDt52wslGGjIqVhua7SEW+aGxtDuu+H9arYtYbDKb4c3p8igf3jbQgNyIOumSf8qtWaiNqleBel0AwaaPZHqzZHFSuiSNN9q1G8+WxVGxeoE6YwKSCFJGD3yEuL/avAQ0Y17DdSD1qfcD9TbMPsBy7csAVjFbmApRZZizFLAYmvOqIApaAfz5cYCJcyDcSrBEoqxCBj1gdYdoK7fQYAhV4OOTyHcgKXjUSg/cz9w70mYY5JuOP09ClAJS5gIVDAQJqk6F6hg3sXwjdeC1m3od1VXD9F1BZP8KOigQ5Kj4UgHBsjr6czRcMlL8CjQ0cD5f02igjMZyn1LdN2wWK/GoSFmwFZkKmUAczAXGBG+oZlqmRIJRr9qWxkg2aNAcTioCTl2JIxTZU3IseO1wNgRoizTz7aD7pOMAVuBZUWmn31DYyaVYM2bkISAAgW1SxEq/O1JGLA5mMkpoJ/WLF23KI0NuoOGrjNWrdMmyLdAWxl/XeMlWD4FJcfAdNrKnAZoFcwICXpNxkCHINiOc/NiqTScQe7d1Q6Z3UlpUrMg54uVQb2K3cKzqAV8vTIVXdcQciQMNGSGFJCwkDaYlIqPSDR9dTR1JNxREhCbo5DTgGBA1+qe8xyBIcx2336Iaj6CpqlbHb+FCdSCpfvXW2AIU9Cdr+t1dwBQoKGaH4fHYJy2UMmb+OW2GZqnZogpKIYiEJmLtHrcMGmIzEOeABdCJXTlOeci0IBIKMtAGAkTEUcFngJDIdO9Ds+B+UhEwCoRRsyOiIFqeBMlPsU7YU2nY0tLYTlAjJgB0wKVTdqosF1AfD5LUWBM6Zycc6NsHhS6UU0RUbAMtGT1s0MdbamITTVbjAJmiW3hkXKUJpen1WhHaodPKQWawq57bmgV9AH7eBisELgsc5T0u2k84g8a7UHF8whlqn1/iG+Kg6I3X8fUDdocfzpqD/0WqmQXtWlwfeh7BI00JJ/C5mRYDLwXSYFvJLeVweQv/meRNBJ/pMsdW4LnEZ59CdySw0fQCW+Mh0i37CXY0v2jTRiyF1pbU+cGNMN3z8keeC0UcQt13BzBgTfGRXsxaPkrLColwh6rPHclaNccBRaObE0LWZburw3Iuea5/TaWMMEj5kvQ+jAD1/4NnhH4HgoPOeEoFNPtU9nEVqMh1y+QZuAZge+BnD6OZ6QVYyMY+NexhgRFustKVbE8CdcsBfiTphcMrb47KybhdU3zOPZuH9JmgOClwq1PoumOez00CteOuqE3wB8Ek9uYchx16GFFt3dU5MY9vEUB3A5VQg6wFQ39LnkdCinwzDzIefQKNYg2KUX6Azz7234DkKehrrvyw0RWn1CXbQWcv0dE/HAnYy/sJO7SXfgBEzSxQmUC1BjY97vXCQljmgJrQHOsINcMiLjnPjAISMWWHcwEk62vpGiOXSsh5Gs95/I4UBCbOaEwHtQBMYgtxiwYIHC5FoY17ZlS2B+FkAL8d5GQ6A4rMQjuqBBhDDl/NwIKliAFE4oCIsphhcK5jhmtExS47pu0Y6YFjgJwtfY3pKBHSyTXCIREwsEityYVWi62Q0ID10wCy8XeTGIFzBgaXXrUsYLEmhE3SDqLKArAClY46thjE1Mb21lIMp7qhPvDLRJ/u1PtOTQLg2pRYAUdv4/YqIIswUsVSXkpmiM8qMQqOJICd6beVooUHgkO3akdrvBwD8O4iw0x5Ain/WV2VAizqVDDKFgpBcOKKQ/mjed9CeeGFQqKJ3gZR/Y4igI8iCMn6LvQ3X+QM9cdxKB8pHcZ0vEohEEJr1gIwzRqmJMgCrqjFMwc2AzDieIlDnX8vIV9V4OQj3uQ6uKPEE4C2mTqFkGBoruPjL0FosUWATyP7xdyTbwcIByw1+fqzP1I8xZ1XZJEN8j8xRL8mmIYIwW7CkGG6plJ093IqOEsYkDmt15m0XF3QrxUVmevyyjw1mqNuZsVDKvlIlPy9hzmreZcx5kTOdM8F+3kPja86jk5Sl7McGrpNrzqeZDh+vk7h8DbaJZH0uim6aVR9BrE8gsvjRt/PVdZiYIgPWvdjJuusNaQ4sDwlWw0fQltaq1peiu56t8b36h7dHmq4Uu48eJPqJDOLQM9hHHZYllqRSx1mZpnNAXGlJVe7VM3cEtJZiHIr/aYqiW/lAzjA5yXOCASQpqDhsWVA+jFcJ3WL5oCxerRaXqrz4hglvtjrjXGq3MFB2NGZR/lKZMqgiCG0lIIkttAaQ49hgLKbGHf9TZlKQWKYZFdqPMizHk4VlWug46USjjOjR5fdtIQEf1vTSLkwisEF0QqoaHeEoeCtgHWxQ1Ue3Iz6Zshu3un6J1lfdmRbSi4mkzrroTqdVuB6DJQd+xIqDZZZ+mLQUXXkbTGj3D9FM3wpveo80wIkBgBlY+5JWSkGYjevqT2OhEybTUo9bzrummaMANUY7YEQzFpEeQNhiPBQjABngq63YBJ1rQoCbZ6hh1VqGUanJ77mMiNV9Gn0o0QO1ZJtzFsne8ibMO8k7egzfrS64oRJYGti7J4lD6P6lVdygFqybebrF5qKN1ust1sX8oBalxLJRiziHEEjiow4OvllH52DinmwK3uANXsANbMnrpdCQdOmteyJBw4K0I+OIQwtLJ4a9uBKd1L8uxA+DxOBkZCDQ28Ql0KSTLdrWnJxjAOhC3hxjDemrbXAiIJurs1zQfIUAJXV4ZQhAVYyDsmUhZs3ptTz800dbALWmCCUJBVHAq9IFYVDIPe9zK+hgLbqn8Ewo6x4Dhp7O6GCM0+vzmkIWJrpgNsAlpEslStARqYRB7QeOZJ0NA89NRLQAJ1RqQCSNCJHa5RD5IwjX3SJtVhtkot1KPS0XKFDjN27BlQkeZ6TsdSA5l0Sr3s05HOQs9UsledcBKos0ipRpeRYKIJlRGPn1kJfbhgKMK4awdT3TIMSzeRUeE2t8qdHnKW+4ZTxkfTNhdqG0XFa8CyA/8jL/1pQEgwh1zCVq3by0jTlzArcWn9qDTzVbAlzJfc+rc5NEMJaCDaQZLgb704rNUqpVuB9ZRvOsVBbVBpPwlSjdG4VKnVBsV6U7A6v15ObAnDiVxCrdIeCyS0xm1XQudGIKFxiyUsVzlwlyBBggQJEiRIkOAX439SmLlxmM8qGwAAAABJRU5ErkJggg=="
                  alt="header"
              /></a>
              <button
                class="navbar-toggler"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent"
                aria-expanded="false"
                aria-label="Toggle navigation"
              >
                <span class="navbar-toggler-icon"></span>
              </button>
              <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0 align-items-center">
                  <li class="nav-item">
                    <a class="nav-link font-primary fw-bold me-4" href="#">Products</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link font-primary fw-bold me-4" href="#"
                      >Why IM3 <br />
                      Ooredoo</a
                    >
                  </li>
                  <li class="nav-item">
                    <a class="nav-link font-primary fw-bold me-4" href="#">Shop</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link font-primary fw-bold me-4" href="#">myIM3</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link font-primary fw-bold me-4" href="#">Buy SIM Card</a>
                  </li>
                  <span class="badge text-bg-danger">BARU</span>
                </ul>
                <form class="d-flex" role="search">
                  <input type="text" class="form-control rounded-pill form-header" />
                </form>
              </div>
            </div>
          </nav>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6 col-7 padding-50">
          <h1 class="fw-bold mb-xl-5 mb-4">
            Upgrade <span class="font-primary">Prime</span>
            via Online Now with nation-wide delivery
          </h1>
          <div class="row mb-xl-5 mb-4">
            <div class="col-xl-6 mb-md-3 mb-0" v-for="data in header" v-bind:key="data.id">
              <MoleculeGrid v-bind:data="data" />
            </div>
          </div>
          <AtomButton class="mb-4" :link="{ name: 'Order Now', url: '#' }" />
        </div>
        <div class="col-md-6 col-5 d-flex justify-content-center align-items-end">
          <img src="../../assets/images/postpaid_person.webp" alt="icon postpaid" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AtomSubtitle from "../atoms/AtomSubtitle.vue";
import AtomButton from "../atoms/AtomButton.vue";
import MoleculeGrid from "../molecules/MoleculeGrid.vue";

export default {
  components: {
    AtomSubtitle,
    AtomButton,
    MoleculeGrid,
  },
};
</script>

<style scoped>
.header {
  background-color: #fed701;
}
.navbar-brand img {
  height: 45px;
  width: 100%;
  object-fit: cover;
}
.form-header {
  width: 198px;
}
.padding-50 {
  padding-bottom: 50px;
  position: relative;
  z-index: 9;
}
@media only screen and (max-width: 992px) {
  .img-premium {
    width: 100%;
  }
}
</style>
