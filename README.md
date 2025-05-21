# scrill-for-mayor
HP-Scrill-For-Mayor
{
  "artist": "Scrill 4 Mayor",
  "track": "Outside",
  "post_text": "Scrill 4 Mayor came *Outside* with a track that feels like narration straight from the pavement. Gritty, real, and unapologetically Detroit.",
  "tags": [
    "#IndieOverIndustry",
    "#Reality2Reel",
    "#Scrill4Mayor",
    "#DetroitMusic",
    "#IndieHipHop",
    "#UndergroundVibes",
    "#OutsideTheIndustry"
  ],
  "article_url": "https://www.reality2reel.net/home/2022/11/28/scrill-4-mayor?rq=scrill"
}
import json

def generate_post(filename):
    with open(filename, 'r') as file:
        data = json.load(file)

    caption = f"""🎤 **{data['artist']}** came *{data['track']}* with a track that feels like narration straight from the pavement.  
{data['post_text']}

🔗 Read more: {data['article_url']}
📍 {' '.join(data['tags'])}
"""
    print(caption)

# Example usage
# generate_post('artist-data/scrill4mayor.json')
# Reality2Reel Automation

This repo contains data files, social media caption templates, and automation scripts for managing Reality2Reel content.

## Structure
- `artist-data/`: JSON profiles of featured artists
- `automation-scripts/`: Python scripts for generating social media posts
- `web-assets/`: Custom site styles or embeds
- `magazine-layouts/`: Magazine issue drafts

## Usage
To generate a social post:
1. Add artist JSON in `artist-data/`
2. Run `generate_post.py` to print the caption
cd path/to/reality2reel-automation
python automation-scripts/generate_post.py
