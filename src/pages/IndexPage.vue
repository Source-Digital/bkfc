<template>
  <q-page class="bg-black text-white">
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">GET READY FOR BKFC 52 ON OCTOBER 20</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 400px"
        v-for="item in getReadyForBKFC52Feed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">UPCOMING EVENTS</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in upcomingFightsFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">LIVE EVENTS</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in liveEventsFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">GET READY FOR BKFC THAILAND 5 NOV 4TH</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in BKFCTHAILANDFEED"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">PROSPECTS: THE NEW GENERATION</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in PROSPECTSFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">KNUCKLE UP AND THROW DOWN!</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in knuckleUpThrowDownFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">BEST OF BKFC HEAVYWEIGHT FIGHTS</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in bestOfHeavyWeightsFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">BRUTAL BKFC BEATDOWNS</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in brutalBeatdownFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">EPIC WOMEN WARS</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in epicWomenFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">FEATURED BKFC LIGHTWEIGHT FIGHTS</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in lightweightFightsFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
    <div class="row q-px-md q-pt-md">
      <div class="col">
        <div class="row">
          <div class="col text-h6">BEST OF FEATHERWEIGHT FIGHTS</div>
        </div>
      </div>
    </div>
    <div class="row no-wrap overflow-auto">
      <q-card
        dark
        class="q-ma-md"
        style="min-width: 300px"
        v-for="item in featherweightFeed"
        :key="item.id"
      >
        <q-img :src="item.media_group[0].media_item[0].src" />
        <div class="row q-px-sm">
          <q-expansion-item
            switch-toggle-side
            expand-separator
            :label="item.title"
          >
            <div class="row">
              <div class="col-auto text-bold">Title:</div>
              <div class="col-auto q-pl-sm text-wrap">{{ item.title }}</div>
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">VideoURL:</div>
              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.content.src)"
                >Click to Copy URL</q-btn
              >
            </div>
            <div class="row items-center">
              <div class="col-auto text-bold">ImageURL</div>

              <q-btn
                dense
                class="col-auto q-pl-sm"
                @click="copyToClipboard(item.media_group[0].media_item[0].src)"
                >Click to Copy URL</q-btn
              >
            </div>
          </q-expansion-item>
        </div>
      </q-card>
    </div>
  </q-page>
</template>

<script setup>
import { ref, onMounted } from "vue";
import axios from "axios";
import { copyToClipboard } from "quasar";

let getReadyForBKFC52Feed = ref([]);
let PROSPECTSFeed = ref([]);
let knuckleUpThrowDownFeed = ref([]);
let bestOfHeavyWeightsFeed = ref([]);
let brutalBeatdownFeed = ref([]);
let epicWomenFeed = ref([]);
let lightweightFightsFeed = ref([]);
let featherweightFeed = ref([]);
let upcomingFightsFeed = ref([]);
let BKFCTHAILANDFEED = ref([]);
let liveEventsFeed = ref([]);

function getURL(payload) {
  copyToClipboard(payload)
    .then(() => {
      // success!
    })
    .catch(() => {
      // fail
    });
}

function getReadyForBKFC52() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=4454&leagueCode=BKFC&teamCode=BKFC&title=GET+READY+FOR+BKFC+52+ON+OCTOBER+20"
    )
    .then((response) => (getReadyForBKFC52Feed.value = response.data.entry));
}

function PROSPECTS() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=4330&leagueCode=BKFC&teamCode=BKFC&title=PROSPECTS%3A+THE+NEW+GENERATION"
    )
    .then((response) => (PROSPECTSFeed.value = response.data.entry));
}

function knuckleUpThrowDown() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=4327&leagueCode=BKFC&teamCode=BKFC&title=KNUCKLE+UP+AND+THROW+DOWN%21"
    )
    .then((response) => (knuckleUpThrowDownFeed.value = response.data.entry));
}

function bestOfHeavyWeights() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=4292&leagueCode=BKFC&teamCode=BKFC&title=BEST+OF+BKFC+HEAVYWEIGHT+FIGHTS"
    )
    .then((response) => (bestOfHeavyWeightsFeed.value = response.data.entry));
}

function brutalBeatdown() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=4144&leagueCode=BKFC&teamCode=BKFC&title=BRUTAL+BKFC+BEATDOWNS"
    )
    .then((response) => (brutalBeatdownFeed.value = response.data.entry));
}

function epicWomen() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=3528&leagueCode=BKFC&teamCode=BKFC&title=EPIC+WOMEN+WARS"
    )
    .then((response) => (epicWomenFeed.value = response.data.entry));
}

function lightweightFights() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=3664&leagueCode=BKFC&teamCode=BKFC&title=FEATURED+BKFC+LIGHTWEIGHT+FIGHTS"
    )
    .then((response) => (lightweightFightsFeed.value = response.data.entry));
}

function featherweightFights() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=3863&leagueCode=BKFC&teamCode=BKFC&title=BEST+OF+FEATHERWEIGHT+FIGHTS"
    )
    .then((response) => (featherweightFeed.value = response.data.entry));
}

function upcomingFights() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/live/277?leagueCode=BKFC&status=upcoming&teamCode=BKFC&title=Upcoming+Events"
    )
    .then((response) => (upcomingFightsFeed.value = response.data.entry));
}

function BKFCTHAILAND() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/marketing/277?id=4555&leagueCode=BKFC&teamCode=BKFC&title=Get+Ready+for+BKFC+Thailand+5+on+Nov+4"
    )
    .then((response) => (BKFCTHAILANDFEED.value = response.data.entry));
}

function liveEvents() {
  axios
    .get(
      "https://applicaster-api.fanreachdata.io/applicaster/live/277?leagueCode=BKFC&status=live&teamCode=BKFC&title=Live+Events"
    )
    .then((response) => (liveEventsFeed.value = response.data.entry));
}

onMounted(async () => {
  getReadyForBKFC52();
  PROSPECTS();
  knuckleUpThrowDown();
  bestOfHeavyWeights();
  brutalBeatdown();
  epicWomen();
  lightweightFights();
  featherweightFights();
  upcomingFights();
  BKFCTHAILAND();
  liveEvents();
});
</script>
