# Sample app: Setup GA4 in your Roku app

> This project was created in an instant with with `npx create-roku-app`. Check it out! https://github.com/haystacknews/create-roku-app

This sample project showcases how to use the library [`vixtech/roku-google-analytics-4`](https://github.com/vixtech/roku-google-analytics-4) to send events to GA4 from your Roku apps. It also includes:

- How to enable Debug Mode

- How to send campaign data (UTM params)

Check the full details in this blogpost: https://arturocuya.com/posts/using-ga4-in-roku

## Building this sample

1. Clone this repository and run `pnpm install`. If you're using `npm`, delete `pnpm-lock.yaml` and run `npm install`.

1. Create a copy of `bsconfig.example.json` and name it `bsconfig.json`. Edit it to set the password for your Roku device.

1. Go to `src/source/utils/ga4.bs` and replace the string `"<your-measurement-id>"` with your measurement id (starts with `G-`).

1. If you're using VSCode (recommended), make sure you have the [BrightScript Language](https://marketplace.visualstudio.com/items?itemName=RokuCommunity.brightscript) plugin installed. Go to the `Run & Debug` panel and launch the app from there.

1. If you're not using VSCode, run `npm run build`, zip the contents of `dist/build` and sideload the app from your Roku's IP website using the browser of your preference.
