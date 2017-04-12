# coinspot-php-client
API client for coinspot.com.au written in PHP

    $coinspot = new Coinspot($key, $secret);

    $coins = ['btc', 'eth', 'xrp', 'ltc', 'dash', 'xmr', 'etc', 'xem', 'rep', 'maid', 'zec', 'doge', 'fct', 'ppc', 'nxt'];
    $results = [];

    foreach ($coins as $coin) {
      $results[$coin] = $coinspot->buyQuote($coin, 1);
      sleep(1);
    }

    var_dump($results);
