# **Solder Reflow Plate**

一個有空就會更新的回流焊加熱台專案

## As Seen On GreatScott! 

This project has recently featured on a DIY or BUY GreatScott! video.

Check it out here - [The Best way to reflow solder? Hot Plate to the rescue! DIY or Buy](https://www.youtube.com/watch?v=QarizoUnRfk)

## UPDATE!!!

基於3.0版本更新了3.1版本，主要差異在於:

- 使用Type-C接口經過USB Power Delivery(PD)取得12V電壓，並透過CH224K晶片實作該協定。
- 加入LED電源燈，可以藉由燈光判斷PD協定的狀態。
- 在MOSFET汲極(Drain)加入10x10(mm)的散熱區域
- 將V3.0中原有的D1二極體PESDMC2FD18VB替換成SMAJ18CA，手工銲接會比較容易。
- 將V3.0中原有的AMS1117-5.0封裝由SOT-89替換成SOT-223，比較常見。
- 將ATmega4809去耦電容封裝由原有的0402改為0603，手工銲接會比較容易。
- 將兩顆按鈕的下拉電容封裝由原有的0402改為0603，手工銲接會比較容易。
- 將兩顆按鈕改為6x6(mm)的貼片元件，比較常見且價格比較便宜。
- 將加熱區背面加上鋪銅，使得熱量更加均勻分布。
- 溫度可以設定到250度，但實際上取決於你的電源供應器

## 未來展望
- 將PD電源改為20V，發揮電源供應器的潛力。
- 將AMS1117改為DC-DC buck，進而降低發熱，追求更高的能量轉換效率。
- 將微控制器改為ESP-12F模組，手工銲接會更加方便。
- 將溫度感測器改為SHT20之類的，這樣可以和OLED模組一起使用I²C介面。
- 降低給微控制器電源的漣波
- 降低MOSFET的峰值，或許更換SMAJ18CA可以改善。
- 改進韌體中按鈕體驗。
- 改變韌體中溫度的byte資料型態，使其超過255度
- 或許可以將加熱板與控制器解耦合，做成模組化，方便更換加熱板，但目前使用起來壽命似乎沒問題。

## Versions

- 70mm x 50mm (Ver 2.4)
  - 12VDC (5A Minimum)
  - 5.5mm x 2.5mm Barrel Jack
  - 0.91" OLED Display
  - ATmega328p Microprocessor

- 70mm x 50mm (Ver 3.0) **NEW**
  - 12VDC (5A Minimum)
  - 5.5mm x 2.5mm Barrel Jack
  - 0.91" OLED Display
  - ATmega4809 Microprocessor

## About the Project

Like any good nerd does I've been expanding my hobby horizons.
I've gone from breadboard, to perf board, through-hole, to SMD, ever increasing circuit complexity and improving my knowledge.
But I've become frustrated with the difficulty of SMD soldering.
Regular soldering jogs small components and needs lots of flux.
Hot air damages plastics.
Hot plates are expensive and can be big wastes of space.

*"But you're a nerd"* I hear you cry, *"why don't you DIY a solution?"*.

[Electronoobs](https://www.youtube.com/channel/UCjiVhIvGmRZixSzupD0sS9Q) shows a great DIY solution using an old clothes iron hot plate.
You can watch his video [here.](https://www.youtube.com/watch?v=C7blZigaaaA)
Have a go!

While I love this solution, I wanted to develop something smaller and more permanent.
Hence the Solder Reflow Plate was born, a PCB-based, MOSFET controlled heater, perfect for easily reflowing SMD components giving surprisingly professional results. Furthermore, these results are achieved without breaking the bank or taking up an enormous amount of desk space.

And so, this nerd bestows upon the world his project, fully open-source and hackable.
Here's hoping that it may be used to develop skills, build custom circuit boards, and make quality designs possible to all!

## Purchase

- Register your email address at [www.solderreflowplate.co.uk](https://www.solderreflowplate.co.uk) to know when it is available to buy!
- There is a worldwide shortage of ATmega328p Microcontrollers. I'm currently working on a small redesign for a more readily available chip.
- Purchase will be available soon!

## License

All parts of this project are covered by a [MIT license](LICENSE).
That means it is entirely open-source, so you get access to everything! (just without warranty or liability)
Feel free to download, customise, hack, and commercialise to your nerdy heart's content.

Want the **easy** life?!
**Purchase** the default design above!
Its fully functional, cheaper than customising, and helps to feed the creator's caffeine addiction 🙃
