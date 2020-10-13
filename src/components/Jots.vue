<template>
  <div id="jots">
    <h2>
      Hi {{user.name}}&mdash;have any thoughts to share?
    </h2>
    <div v-for="jot in jots" v-bind:key="jot.id" class="jot">
      <div>{{jot.time}}</div>
      <p>{{jot.msg}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Jots',
  props: ["user"],
  data() {
    return {
      jots: [
        {
          id: "dc6854c0-f556-459b-8e55-c4d97971ede3",
          msg: "Is it more important for something to be customer-directed? What does the buzzword 'technologies' really mean? It is pushing the envelope At the end of the pudding is in the industry, but our one-to-one, customer-defined, robust C2C2C M&A and user-proof use. We will enlarge our ability to whiteboard without lessening our aptitude to evolve without decreasing our power to benchmark. The capacity to enable perfectly leads to the capacity to harness without devaluing our power to deliver. Without C2C, you will lack architectures. We will augment our aptitude to disintermediate. Helping marketers serve unmatched cross-phase personalized experiences at every step of the pudding is in the industry, but our C2C2C paradigms and easy configuration is usually considered an amazing achievement.",
          time: "2020-10-12T18:04:54.724",
          done: true
        },
        {
          id: "ca2b47a9-a8f8-4b0d-a990-182c1fd29017",
          msg: "It sounds wonderful, but it's 100 percent accurate! The experiences factor is short-term. Without development, you will lack experiences. Without niches, you will lack affiliate-based compliance. If you productize globally, you may also reintermediate magnetically. Without efficient, transparent bloatware, you will lack social networks. Without niches, you will lack affiliate-based compliance. Our functionality is unparalleled, but our plug-and-play re-purposing and easy configuration is frequently considered a terrific achievement. Without micro-resource-constrained performance, you will lack research and development. Without micro-resource-constrained performance, you will lack research and development.",
          time: "2020-10-12T18:12:04.529",
          done: true
        },
        {
          id: "6ddf31ec-0e6a-45dd-bf71-ad965cf11b42",
          msg: "Without efficient, transparent bloatware, you will lack social networks. We will revalue our aptitude to disintermediate. Clicking on this link which refers to B2B Marketing awards shortlist will take you to the capacity to harness without devaluing our capability to upgrade. It sounds wonderful, but it's 100 percent accurate! The experiences factor is compelling. Without niches, you will lack architectures. Imagine a combination of IIS and J2EE. Do you have a virally-distributed plan of action for managing emerging partnerships? Without data hygiene supervising, you will lack social networks. Do you have a virally-distributed plan of action for managing emerging partnerships? Without data hygiene supervising, you will lack cross-media CAE.",
          time: "2020-10-12T18:18:15.798",
          done: false
        },
        {
          id: "4f27dd71-1711-42e6-a967-d64dab5a9221",
          msg: "Our infinitely reconfigurable feature set is unparalleled in the industry, but our granular integrated, value-added convergence and easy use is frequently considered a remarkable achievement taking into account this month's financial state of things! If all of this may seem marvelous, but it's realistic! Imagine a combination of ActionScript and PHP. Quick: do you have a plan to become customized. What does the commonly-accepted commonly-accepted standard industry term 'back-end'. Without C2C, you will lack cross-media CAE. Our functionality is unparalleled, but our newbie-proof administration and simple configuration. Have you ever been unable to disintermediate your feature set? In one step? What do we transform? Anything and everything, regardless of humbleness! What does it really mean to target 'micro-efficiently'? It may seem confusing, but it's accurate! We will revalue our aptitude to disintermediate.",
          time: "2020-10-12T18:27:23.735",
          done: false
        },
        {
          id: "27ec9e23-0305-4b7c-8192-6721eac2f5e0",
          msg: "Without niches, you will lack affiliate-based compliance. What do we transform? Anything and everything, regardless of incomprehensibility! We understand that if you incentivize dynamically, you may have to synergize wirelessly. Without macro-vertical CAE, you will lack synergies. Without interfaces, you will lack affiliate-based compliance. Quick: do you have a plan to become cross-media? We think that most efficient web-based applications use far too much Perl, and not enough HTTP. Our end-to-end feature set is unmatched in the industry, but our plug-and-play re-purposing and easy configuration is usually considered an amazing achievement. Imagine a combination of Perl and FOAF. What does the commonly-accepted commonly-accepted standard industry term 'back-end'.",
          time: "2020-10-12T18:31:04.847",
          done: false
        },
        {
          id: "80cf8d9d-e089-45b4-a439-ed9bb04922dd",
          msg: "A company that can streamline elegantly will (at some unspecified point in the future) be able to transition easily. Our infinitely reconfigurable feature set is unparalleled, but our sexy raw bandwidth and easy operation is invariably considered a remarkable achievement taking into account this month's financial state of things! If all of this comes off as mixed-up to you, that's because it is! If you target efficiently, you may also reintermediate magnetically. A company that can streamline elegantly will (at some undefined point of time in the future) be able to engineer seamlessly.",
          time: "2020-10-12T18:33:46.358",
          done: false
        }
      ]
    }
  }
}
</script>

<style scoped>
* {
  text-align: justify;
}
h2 {
  margin: 2em 0;
  font-weight: 200;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
#jots {
  max-width: 1080px;
  margin: 0 auto;
}
.jot {
  margin-bottom: 32px;
}
</style>
