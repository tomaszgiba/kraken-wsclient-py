# Kraken WebSockets Client in Python

Sample Kraken WebSockets client in Python.  This client was created for
demonstration purposes only.  It is neither maintained nor supported.

## Installation

    pip install kraken-wsclient-py

## Sample Usage

    from kraken_wsclient_py import kraken_wsclient_py as client

    def my_handler(message):
        # Here you can do stuff with the messages
        print(message)

    my_client = client.WssClient()
    my_client.subscribe_public(
        subscription={
            'name': 'trade'
        },
        pair=['XBT/USD', 'XRP/USD'],
        callback=my_handler
    )

    my_client.start()


## Compatibility

This code has been tested on Python 3.7.

## Contributing

Pull requests are not monitored and likely will be ignored.

