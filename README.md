# HideText
## Hide and Recover Secret Messages Inside Emoji 🕵️‍♂️
This is a single-page web app for hiding and recovering secret messages inside emoji.
## How It Works
### Encoding Messages
- **Pick an emoji**: The top section lets you pick an emoji from a row of common choices
- **Enter your secret**: You type any message—words, symbols, even multi-line text—into the secret message box
- **Hit Encode**: The app converts your text into UTF-8 bytes
- **Hidden storage**: Those bytes are then stored invisibly using Unicode variation selectors attached to the chosen emoji
- **Invisible result**: The result looks like a normal emoji, but it secretly carries your hidden data
- **Easy sharing**: You can copy this special emoji string with a single click and paste it into any chat or document
### Decoding Messages
- **Reverse process**: The Decode pane works in reverse: paste the emoji string and it reconstructs the original text
- **Clear feedback**: If no hidden data is found, it tells you clearly instead of failing silently
### Additional Features
- **Help section**: Explains the trick, links to the original article, and reminds users that some platforms may strip hidden data
- **Unicode magic**: Uses Unicode variation selectors to invisibly attach data to emoji characters
- **Platform compatibility**: Works across different platforms, though some may strip the hidden data
- **Tested on WhatsApp**: Tested on WhatsApp and it works
## Usage
1. Open the web app
2. Select an emoji from the available options
3. Type your secret message in the input field
4. Click "Encode" to hide your message in the emoji
5. Copy the resulting emoji and share it anywhere
6. To decode, paste an encoded emoji into the decode field and click "Decode"
## Technical Details
The app leverages Unicode variation selectors to invisibly store UTF-8 encoded text data within emoji characters. This creates a steganographic effect where the emoji appears normal but contains hidden information.
⚠️ **Note**: Some platforms and applications may strip or normalize Unicode characters, which could remove the hidden data.
