# srplay-dmenu

# Sveriges Radio dmenu Script

This script combines functionalities for listening to live radio and podcast episodes from Sveriges Radio using `dmenu`. It integrates features from two separate scripts: [srpod-dmenu](https://github.com/nirucon/srpod-dmenu) and [sverigesradio-dmenu](https://github.com/nirucon/sverigesradio-dmenu), providing a unified experience for users.
I use this with my [Arch Linux Post Install script](https://github.com/nirucon/nirucon-alpi) and my [nirucon-suckless-arch](https://github.com/nirucon/nirucon-suckless-arch) setup.

## Features

- **Live Radio Streaming**: Select and stream live radio channels such as P1, P2, P3, P4, and Ekot-direkt.
- **Podcast Search and Playback**: Search for podcast episodes and play them directly.
- **Process Management**: Easily stop the current stream or podcast.

## Dependencies

- `dmenu`
- `mpv`
- `notify-send`
- `jq`
- `curl`

## Installation

1. Clone this repository and move it to /usr/local/bin:
   ```sh
   git clone https://github.com/nirucon/srplay-dmenu
   cd srplay-dmenu
   chmod +x srplay-dmenu
   sudo cp srplay-dmenu /usr/local/bin
   ```

2. Ensure all dependencies are installed:
   ```sh
   sudo pacman -S dmenu mpv notify-send jq curl
   sudo apt-get install dmenu mpv notify-send jq curl
   ```

## Usage

Run the script from dmenu or your terminal:
```sh
./srplay-dmenu
```

A menu will appear in dmenu with the following options:
- **Search Podcast**: Enter a search term to find and play podcast episodes.
- **Turn off current pod**: Stop the currently playing podcast.
- **SR Live radio**: Select a live radio station to stream.
- **Exit**: Exit the script.

## Notes

This script is a combination of two other scripts by Nicklas Rudolfsson:
- [srpod-dmenu](https://github.com/nirucon/srpod-dmenu)
- [sverigesradio-dmenu](https://github.com/nirucon/sverigesradio-dmenu)

## License

Feel free to use and modify, buy me something if you want ;)
