## Privacy-Preserving Tor Network Measurements

This page provides details about a small, short-term, safe, and secure measurement study of the usage of the [Tor](https://www.torproject.org) network. In particular, we aim to measure:
* popularity of countries and autonomous systems accessesing Tor Guards,
* connection lifetime to Tor Guards,
* popularity of web domains accessed via Tor Exits,
* usage, failure rates, and popularity of Tor Onion Services,

while providing strong user privacy guarantees.

We believe that this study is safe: we only learn total counts or a histogram of counts, with added noise. Because we use PrivCount, we do not learn the usage of single relays, or total network usage without any noise. All unblinded data is kept on the collecting relay, and is automatically destroyed after processing. See the [safety section](#what-are-we-doing-how-is-this-safe) for more details.

### Who are we?

We plan to list our names, affiliations, and contact info here soon. However, this measurement study is part of a larger research paper; most research conferences require submission without author attribution in order to avoid introducing biases into the paper review process. We link to this page in our paper, and so listing our names here could be grounds for immediate rejection. We plan to add our names, affiliations, and email addresses here once our paper clears the submission process.

That being said, you can contact the people operating the relays used in this study by following the links in the relay section below, and if you click around enough you may be able to find the github repository maintainer. Program committees should avoid searching too hard in order to preserve the integrity of the review process.

### What is the general idea?

We are working on understanding the usage of the Tor network:
* where clients access the network from, and for how long,
* where clients go when they access Internet sites,
* where clients go when they access Onion sites, and how well that works.

### What are we doing? How is this safe?

Our measurement study explicitly **prioritizes user safety as a primary goal**. We practice data minimization, limit measurement granularity, and provide additional security to the measurement process as described below. We have incorporated feedback from the [Tor Research Safety Board](https://research.torproject.org/safetyboard.html) into our methodology.

### Which relays are involved in the measurement?

The following relays are part of our PrivCount deployment. The data collected by these relays is blinded and securely aggregated while also being protected by differential privacy. Each individual relay learns nothing except the final combined results from all relays.

  - [09FA8B4F665AD65D2C2A49870F1AA3BA8811E449](https://atlas.torproject.org/#details/09FA8B4F665AD65D2C2A49870F1AA3BA8811E449)
  - [068308AD070849A71B8C1DB06C2509E82C40B908](https://atlas.torproject.org/#details/068308AD070849A71B8C1DB06C2509E82C40B908)
  - [335746A6DEB684FABDF3FC5835C3898F05C5A5A8](https://atlas.torproject.org/#details/335746A6DEB684FABDF3FC5835C3898F05C5A5A8)
  - [363F42695F2DD825DA5A4E6ABF3FBDFCFD1E9AE2](https://atlas.torproject.org/#details/363F42695F2DD825DA5A4E6ABF3FBDFCFD1E9AE2)
  - [B6718125C43ECA2E5011B3C681BB6638617A9686](https://atlas.torproject.org/#details/B6718125C43ECA2E5011B3C681BB6638617A9686)
  - [C6B3546CC6BCCB649FEC82D348D464554BC6323D](https://atlas.torproject.org/#details/C6B3546CC6BCCB649FEC82D348D464554BC6323D)
  - [12B80ABF019354A9D25EE8BE85EB3C0AD8F7DFC1](https://atlas.torproject.org/#details/12B80ABF019354A9D25EE8BE85EB3C0AD8F7DFC1)
  - [DE684E6C6B7773B8BE74B4D941E4178988E15E26](https://atlas.torproject.org/#details/DE684E6C6B7773B8BE74B4D941E4178988E15E26)
  - [4B1E3276137AD12DCCEBE354EA11C1E47F804F67](https://atlas.torproject.org/#details/4B1E3276137AD12DCCEBE354EA11C1E47F804F67)
  - [C170AE5A886C5A09D6D1CF5CF284653632EEF25D](https://atlas.torproject.org/#details/C170AE5A886C5A09D6D1CF5CF284653632EEF25D)
  - [A5945077E0D35729F8E2920A54BE12A0058B403E](https://atlas.torproject.org/#details/A5945077E0D35729F8E2920A54BE12A0058B403E)
  - [0DA9BD201766EDB19F57F49F1A013A8A5432C008](https://atlas.torproject.org/#details/0DA9BD201766EDB19F57F49F1A013A8A5432C008)
  - [D53793315E290D250E9AFC431A4C9068A1E53C98](https://atlas.torproject.org/#details/D53793315E290D250E9AFC431A4C9068A1E53C98)
  - [11EAB5C9137906EF7E6A32365C4B37613698E647](https://atlas.torproject.org/#details/11EAB5C9137906EF7E6A32365C4B37613698E647)
  - [91516595837183D9ECD1318D00723A8676F4731C](https://atlas.torproject.org/#details/91516595837183D9ECD1318D00723A8676F4731C)
  - [1A4488A367D89D0EFDA88116059FEBCACF0F508A](https://atlas.torproject.org/#details/1A4488A367D89D0EFDA88116059FEBCACF0F508A)
  - [98D10461F6EDF13780D20D7E402E67F40C5ADBD9](https://atlas.torproject.org/#details/98D10461F6EDF13780D20D7E402E67F40C5ADBD9)

### What is the measurement status?

We will be collecting periodic measurements from 8 December 2017 through February 2018.
