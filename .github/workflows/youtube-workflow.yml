name: Latest YouTube Videos
on:
  schedule:
    # Runs every hour
    - cron: '0 * * * *'
  workflow_dispatch:

jobs:
  update-readme-with-youtube:
    name: Update this repo's README with latest videos from YouTube
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: gautamkrishnar/blog-post-workflow@master
        with:
          comment_tag_name: "YOUTUBE"
          feed_list: "https://www.youtube.com/feeds/videos.xml?channel_id=UCDCHcqyeQgJ-jVSd6VJkbCw"