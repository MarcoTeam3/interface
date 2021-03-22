<template>
  <v-app>
    <v-container class="grey lighten-5">
      <v-row class="mb-6" no-gutters>
        <v-col>
          <v-card elevation="16" max-width="350" class="mx-auto">
            <v-card-title class="white--text teal lightning-4">
              {{ title }}
            </v-card-title>
            <v-virtual-scroll
              :bench="benched"
              :items="items"
              height="300"
              item-height="64"
            >
              <template v-slot:default="{ item }">
                <v-list-item :key="item">
                  <v-list-item-action>
                    <v-btn fab small depressed color="success">
                      {{ item }}
                    </v-btn>
                  </v-list-item-action>

                  <v-list-item-content>
                    <v-list-item-title>
                      User Database Record <strong>ID {{ item }}</strong>
                    </v-list-item-title>
                  </v-list-item-content>

                  <v-list-item-action>
                    <v-icon small> mdi-open-in-new </v-icon>
                  </v-list-item-action>
                </v-list-item>

                <v-divider></v-divider>
              </template>
            </v-virtual-scroll>
          </v-card>
        </v-col>
         <v-col>
          <v-card elevation="16" max-width="350" class="mx-auto">
            <v-card-title class="white--text teal lightning-4">
              {{ title2 }}
            </v-card-title>
            <v-virtual-scroll
              :bench="benched"
              :items="items"
              height="300"
              item-height="64"
            >
              <template v-slot:default="{ item }">
                <v-list-item :key="item">
                  <v-list-item-action>
                    <v-btn fab small depressed color="success">
                      {{ item }}
                    </v-btn>
                  </v-list-item-action>

                  <v-list-item-content>
                    <v-list-item-title>
                      User Database Record <strong>ID {{ item }}</strong>
                    </v-list-item-title>
                  </v-list-item-content>

                  <v-list-item-action>
                    <v-icon small> mdi-open-in-new </v-icon>
                  </v-list-item-action>
                </v-list-item>

                <v-divider></v-divider>
              </template>
            </v-virtual-scroll>
          </v-card>
        </v-col>
         <v-col>
          <v-card elevation="16" max-width="350" class="mx-auto">
            <v-card-title class="white--text teal lightning-4">
              {{ title3 }}
            </v-card-title>
            <v-virtual-scroll
              :bench="benched"
              :items="items"
              height="300"
              item-height="64"
            >
              <template v-slot:default="{ item }">
                <v-list-item :key="item">
                  <v-list-item-action>
                    <v-btn fab small depressed color="success">
                      {{ item }}
                    </v-btn>
                  </v-list-item-action>

                  <v-list-item-content>
                    <v-list-item-title>
                      User Database Record <strong>ID {{ item }}</strong>
                    </v-list-item-title>
                  </v-list-item-content>

                  <v-list-item-action>
                    <v-icon small> mdi-open-in-new </v-icon>
                  </v-list-item-action>
                </v-list-item>

                <v-divider></v-divider>
              </template>
            </v-virtual-scroll>
          </v-card>
        </v-col>
         <v-col>
          <v-card elevation="16" max-width="350" class="mx-auto">
            <v-card-title class="white--text teal lightning-4">
              {{ title4 }}
            </v-card-title>
            <v-virtual-scroll
              :bench="benched"
              :items="items"
              height="300"
              item-height="64"
            >
              <template v-slot:default="{ item }">
                <v-list-item :key="item">
                  <v-list-item-action>
                    <v-btn fab small depressed color="success">
                      {{ item }}
                    </v-btn>
                  </v-list-item-action>

                  <v-list-item-content>
                    <v-list-item-title>
                      User Database Record <strong>ID {{ item }}</strong>
                    </v-list-item-title>
                  </v-list-item-content>

                  <v-list-item-action>
                    <v-icon small> mdi-open-in-new </v-icon>
                  </v-list-item-action>
                </v-list-item>

                <v-divider></v-divider>
              </template>
            </v-virtual-scroll>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    benched: 0,
    title: "USG",
    title2: "LIBELLE",
    title3: "CAISSE",
    title4: "MOYEN D'AF"
  }),
  computed: {
    items() {
      return Array.from({ length: this.length }, (k, v) => v + 1);
    },
    length() {
      return 7000;
    },
  },
};
</script>
