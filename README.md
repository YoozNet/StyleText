# PHP Fontify - Text Styler

This is a simple PHP script to convert plain text into various Unicode styles for use in profiles, chats, and social media, without requiring an API.

## Features

- Converts text to multiple styles (bold, italic, underline, etc.)
- Supports various text transformations for easy use in different platforms
- Simple and easy-to-use functions with no external dependencies.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/YoozNet/StyleText.git
   ```
2. Navigate to the project directory:
   ```sh
   cd StyleText
   ```
3. Run the script in a PHP environment.

## Usage
```php
include 'fontify.php';

$text = "hello word";
$styledTexts = convertTextToFonts($text);
print_r($styledTexts);

$num = 1234;
$styledNumberss = convertNumberToFonts($num);
print_r($styledNumberss);

```
### Example Output:
```
Array
(
    [0] => ℌ𝔈𝔏𝔏𝔒 𝔚𝔒ℜ𝔏𝔇
    [1] => 𝐇𝐄𝐋𝐋𝐎 𝐖𝐎𝐑𝐋𝐃
    [2] => ℋℰℒℒ𝒪 𝒲𝒪ℛℒ𝒟
    [3] => 𝗛𝗘𝗟𝗟𝗢 𝗪𝗢𝗥𝗟𝗗
    [4] => 𝖧𝖤𝖫𝖫𝖮 𝖶𝖮𝖱𝖫𝖣
    [5] => ℋℰℒℒ𝒪 𝒲𝒪ℛℒ𝒟
    [6] => 𝙷𝙴𝙻𝙻𝙾 𝚆𝙾𝚁𝙻𝙳
    [7] => ℍ𝔼𝕃𝕃𝕆 𝕎𝕆ℝ𝕃𝔻
    [8] => 𝐇𝐄𝐋𝐋𝐎 𝐖𝐎𝐑𝐋𝐃
    [9] => 𝑯𝑬𝑳𝑳𝑶 𝑾𝑶𝑹𝑳𝑫
    [10] => 𝐻𝐸𝐿𝐿𝑂 𝑊𝑂𝑅𝐿𝐷
    [11] => HELLO WORLD
    [12] => 𝓗𝓔𝓛𝓛𝓞 𝓦𝓞𝓡𝓛𝓓
    [13] => ʰᵉˡˡᵒ ʷᵒʳˡᵈ
    [14] => 𝙃𝙀𝙇𝙇𝙊 𝙒𝙊𝙍𝙇𝘿
    [15] => 𝘏𝘌𝘓𝘓𝘖 𝘞𝘖𝘙𝘓𝘋
    [16] => 𝖧𝖤𝖫𝖫𝖮 𝖶𝖮𝖱𝖫𝖣
    [17] => Ⓗ︎Ⓔ︎Ⓛ︎Ⓛ︎Ⓞ︎ Ⓦ︎Ⓞ︎Ⓡ︎Ⓛ︎Ⓓ︎
    [18] => ᕼᗴᒪᒪO ᗯOᖇᒪᗪ
    [19] => 🅗︎🅔︎🅛︎🅛︎🅞︎ 🅦︎🅞︎🅡︎🅛︎🅓︎
    [20] => ℌ𝔈𝔏𝔏𝔒 𝔚𝔒ℜ𝔏𝔇
    [21] => 𝕳𝕰𝕷𝕷𝕺 𝖂𝕺𝕽𝕷𝕺
    [22] => H͜͡E͜͡L͜͡L͜͡O͜͡ W͜͡O͜͡R͜͡L͜͡D͜͡
    [23] => 𝗛𝗘𝗟𝗟𝗢 𝗪𝗢𝗥𝗟𝗗
    [24] => H̆̈Ĕ̈L̆̈L̆̈Ŏ̈ W̆̈Ŏ̈R̆̈L̆̈D̆̈
    [25] => H̑̈Ȇ̈L̑̈L̑̈Ȏ̈ W̑̈Ȏ̈Ȓ̈L̑̈D̑̈
    [26] => 🇭 🇪 🇱 🇱 🇴  🇼 🇴 🇷 🇱 🇩 
    [27] => 🄷🄴🄻🄻🄾 🅆🄾🅁🄻🄳
    [28] => 🅷︎🅴︎🅻︎🅻︎🅾︎ 🆆︎🅾︎🆁︎🅻︎🅳︎
    [29] => ꫝꫀꪶꪶꪮ ᭙ꪮ𝘳ꪶᦔ
    [30] => 卄乇ㄥㄥㄖ 山ㄖ尺ㄥᗪ
    [31] => H̾E̾L̾L̾O̾ W̾O̾R̾L̾D̾
    [32] => H̥ͦE̥ͦL̥ͦL̥ͦO̥ͦ W̥ͦO̥ͦR̥ͦL̥ͦD̥ͦ
    [33] => H͟E͟L͟L͟O͟ W͟O͟R͟L͟D͟
    [34] => ꀍꏂ꒒꒒ꂦ ꅐꂦꋪ꒒ꀷ
    [35] => H҉E҉L҉L҉O҉ W҉O҉R҉L҉D҉
    [36] => H҈E҈L҈L҈O҈ W҈O҈R҈L҈D҈
    [37] => H̸E̸L̸L̸O̸ W̸O̸R̸L̸D̸
    [38] => H⃠E⃠L⃠L⃠O⃠ W⃠O⃠R⃠L⃠D⃠
    [39] => H̺͆E̺͆L̺͆L̺͆O̺͆ W̺͆O̺͆R̺͆L̺͆D̺͆
    [40] => H͎E͎L͎L͎O͎ W͎O͎R͎L͎D͎
    [41] => ዘቿረረዐ ሠዐዪረዕ
    [42] => H̶E̶L̶L̶O̶ W̶O̶R̶L̶D̶
    [43] => H༙E༙L༙L༙O༙ W༙O༙R༙L༙D༙
)

Array
(
    [0] => 𝟙𝟚𝟛𝟜
    [1] => 𝟏𝟐𝟑𝟒
    [2] => 𝟷𝟸𝟹𝟺
    [3] => ①②③④
    [4] => ➊➋➌➍
)

```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author
Developed by **[YoozNet]**. Feel free to contribute or report issues!

## Contributions
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Contact
For any inquiries, you can reach me at [SaeedShanaqi+github@gmail.com] or open an issue in this repository.
