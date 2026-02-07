- [Cheerio](https://cheerio.js.org/docs/intro)
    - [Traversing](https://cheerio.js.org/docs/basics/traversing)
- [Google Finance](https://www.google.com/finance/quote/MSFT:NASDAQ)

- [Yahoo Finance](https://finance.yahoo.com/quote/NVDA)
    - Quote
        - Path: - /html/body/div[1]/main/section/section/section/article/section[1]/div[2]/div[1]/section/div/section[1]/div[1]/fin-streamer[1]/span
        - <fin-streamer class="livePrice svelte-el7lzh" data-symbol="NVDA" data-testid="qsp-price" data-field="regularMarketPrice" data-trend="none" data-pricehint="2" data-value="887" active=""><span>887.00</span></fin-streamer>
    - Target
        - <fin-streamer data-symbol="NVDA" data-value="852.49" data-trend="none" active="" data-field="targetMeanPrice" class="svelte-tx3nkj">852.49</fin-streamer>
        ```javascript
       $("fin-streamer[data-field='targetMeanPrice'])
        - ```` 
        - #nimbus-app > section > section > section > article > div.container.svelte-tx3nkj > ul > li:nth-child(16) > span.value.svelte-tx3nkj > fin-streamer
        - /html/body/div[1]/main/section/section/section/article/div[2]/ul/li[16]/span[2]/fin-streamer
