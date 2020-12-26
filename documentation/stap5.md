---
layout: page
title: Stap 5 - Betaal met Bitcoin
show_in_menu: false
disable_anchors: true
---

## Betalen met bitcoin

### Kippen voederen
Ga naar [pollofeed](https://pollofeed.com/) en druk op `Click to feed!`. Scan de QR-code of kies `Open in wallet`. Betaal de Lightning-factuur en ga terug naar de website.

### Doneren

<style type="text/css"> .btcpay-form { display: inline-flex; align-items: center; justify-content: center; } .btcpay-form--inline { flex-direction: row; } .btcpay-form--block { flex-direction: column; } .btcpay-form--inline .submit { margin-left: 15px; } .btcpay-form--block select { margin-bottom: 10px; } .btcpay-form .btcpay-custom-container{ text-align: center; }.btcpay-custom { display: flex; align-items: center; justify-content: center; } .btcpay-form .plus-minus { cursor:pointer; font-size:25px; line-height: 25px; background: #DFE0E1; height: 30px; width: 45px; border:none; border-radius: 60px; margin: auto 5px; display: inline-flex; justify-content: center; } .btcpay-form select { -moz-appearance: none; -webkit-appearance: none; appearance: none; color: currentColor; background: transparent; border:1px solid transparent; display: block; padding: 1px; margin-left: auto; margin-right: auto; font-size: 11px; cursor: pointer; } .btcpay-form select:hover { border-color: #ccc; } #btcpay-input-price { -moz-appearance: none; -webkit-appearance: none; border: none; box-shadow: none; text-align: center; font-size: 25px; margin: auto; border-radius: 5px; line-height: 35px; background: #fff; } #btcpay-input-price::-webkit-outer-spin-button, #btcpay-input-price::-webkit-inner-spin-button { -webkit-appearance: none; margin: 0; } </style>
<style type="text/css"> input[type=range].btcpay-input-range { -webkit-appearance:none; width:100%; background: transparent; } input[type=range].btcpay-input-range:focus { outline:0; } input[type=range].btcpay-input-range::-webkit-slider-runnable-track { width:100%; height:3.1px; cursor:pointer; box-shadow:0 0 1.7px #020,0 0 0 #003c00; background:#f3f3f3; border-radius:1px; border:0; } input[type=range].btcpay-input-range::-webkit-slider-thumb { box-shadow:none; border:2.5px solid #cedc21; height:22px; width:22px; border-radius:50%; background:#0f3723; cursor:pointer; -webkit-appearance:none; margin-top:-9.45px } input[type=range].btcpay-input-range:focus::-webkit-slider-runnable-track { background:#fff; } input[type=range].btcpay-input-range::-moz-range-track { width:100%; height:3.1px; cursor:pointer; box-shadow:0 0 1.7px #020,0 0 0 #003c00; background:#f3f3f3; border-radius:1px; border:0; } input[type=range].btcpay-input-range::-moz-range-thumb { box-shadow:none; border:2.5px solid #cedc21; height:22px; width:22px; border-radius:50%; background:#0f3723; cursor:pointer; } input[type=range].btcpay-input-range::-ms-track { width:100%; height:3.1px; cursor:pointer; background:0 0; border-color:transparent; color:transparent; } input[type=range].btcpay-input-range::-ms-fill-lower { background:#e6e6e6; border:0; border-radius:2px; box-shadow:0 0 1.7px #020,0 0 0 #003c00; } input[type=range].btcpay-input-range::-ms-fill-upper { background:#f3f3f3; border:0; border-radius:2px; box-shadow:0 0 1.7px #020,0 0 0 #003c00; } input[type=range].btcpay-input-range::-ms-thumb { box-shadow:none; border:2.5px solid #cedc21; height:22px; width:22px; border-radius:50%; background:#0f3723; cursor:pointer; height:3.1px; } input[type=range].btcpay-input-range:focus::-ms-fill-lower { background:#f3f3f3; } input[type=range].btcpay-input-range:focus::-ms-fill-upper { background:#fff; } </style>
<form method="POST"  action="https://btcpay.bewijsvanwerk.com/api/v1/invoices" class="btcpay-form btcpay-form--block">
  <input type="hidden" name="storeId" value="FHT9sXvdm28YT7JeXdAKrjctx6ZihNf3XnFfVAPp29Mo" />
  <input type="hidden" name="checkoutDesc" value="Doneer aan Bewijs van Werk" />
  <div class="btcpay-custom-container">
    <input id="btcpay-input-price" name="price" type="text" min="0" max="none" step="any" value="3" style="width: 209px;" oninput="event.preventDefault();isNaN(event.target.value) || event.target.value <= 0 ? document.querySelector('#btcpay-input-price').value = 3 : event.target.value" onchange="document.querySelector('#btcpay-input-range').value = document.querySelector('#btcpay-input-price').value" />
    <select name="currency">
      <option value="USD">USD</option>
      <option value="GBP">GBP</option>
      <option value="EUR" selected>EUR</option>
      <option value="BTC">BTC</option>
    </select>
    <input class="btcpay-input-range" id="btcpay-input-range" value="3" type="range" min="1" max="20" step="1" style="width:209px;margin-bottom:15px;" oninput="document.querySelector('#btcpay-input-price').value = document.querySelector('#btcpay-input-range').value" />
  </div>
<button type="submit" class="submit" name="submit" style="min-width:209px; min-height:57px; border-radius: 4px;border-style: none;background-color: #0f3b21;" alt="Pay with BtcPay, Self-Hosted Bitcoin Payment Processor"><span style="color:#fff">Betaal met</span>
<img src="https://btcpay.bewijsvanwerk.com/img/logo.svg" style="height:57px;display:inline-block;padding: 5% 0 5% 5px;">
</button></form>

### Stuur een bericht de ruimte in

Ga naar de website van [Blockstream](https://blockstream.com/satellite-queue/) en geef het bericht in dat je wil versturen.
~~~
Ik stuurde net een bericht de ruimte in - betaald met Lightning.

Ga naar spaartechnologie.com om Bitcoin te leren.
~~~

Kies een fee en betaal de Lightning-factuur.

---

[Verder gaan](stap6.md) --
[Terug naar overzicht](overzicht.md)
