## New Relic Browser Agent Demo Screenshot
![New Relic Browser Agent Logging Demo](/screenshot-min.png?raw=true "Optional Title")

This Browser logging demo focuses on several aspects of the New Relic Browser Agent: `Native Error collection`, `noticeError() collection`, `Browser Console Log collection`, `.log() collection`

# Local Dev Environment

## Pre-Reqs
* New Relic Account
* Apache (or your favorite web server for serving static `html/png/json` files)
* Your favorite IDE for editing `index.html` 

## Installation
 1. Clone or download the `nr-browser-logging-demo` repo to a directory to be served locally from your web server
 2. Create a new `Browser Application` using copy/paste [here](https://onenr.io/0MRNpYqNqQn)
 3. Insert the `browser snippet` from step 2 into the `index.html` file
 4. To customize the header and UI for the demo, replace the `header-min.png` (800px x 200px) with a file of your choice
 5. Edit the `local config options` in the `index.html` file
 6. Load `index.html` locally from your web server and interact; `Browser` and `Log` telemetry will be sent to New Relic
 7. Navigate to the `Browser Application` you created in New Relic (step 2) and browse the Log telemetry from the Demo

## Include Files

This New Relic Browser logging demo includes three files: `index.html`, `ajax.json`, and `header-min.png`.

- `index.html` - NR Browser Agent Script, local config options, and example code to emit logs to New Relic from the browser agent
- `header-min.png` - Header file used for branding the demo
- `ajax.json` - Example JSON file used in the Ajax example; subsequently written to a Log in New Relic from the browser agent

## Troubleshooting
* Don't see any telemetry in New Relic? Ensure you replace the `Step 1 - Insert your NR Browser Agent Script from your demo account (copy/paste method)` in `index.html` with your `Browser Application` using copy/paste [here](https://onenr.io/0MRNpYqNqQn)
* After creating a new Browser Application in New Relic, it might take up to ~20 minutes for [entity synthesis](https://newrelic.com/blog/how-to-relic/entity-synthesis) to occur, so that you'll see the logs from the Demo in context to your browser application.
* Want to see what's happening in the demo? The `local logger` text area will refresh from the actions in the demo, but inspecting the `console` will also expose other information about the logs being sent to New Relic.
