# digitalclash.github.io
digitalclash
$web3Browser.setOnSignMessageListener(new OnSignMessageListener() {
            @Override
            public void onSignMessage(Message<String> message) {
                web3Browser.onSignCancel(message);
            }
        });
        web3Browser.setOnSignPersonalMessageListener(new OnSignPersonalMessageListener() {
            @Override
            public void onSignPersonalMessage(Message<String> message) {
                web3Browser.onSignCancel(message);
            }
        });
        web3Browser.setOnSignTransactionListener(new OnSignTransactionListener() {
            @Override
            public void onSignTransaction(final Transaction transaction) {
                Log.i(TAG, "onSignTransaction 处理交易签名，转账");
            }
        });
        web3Browser.setChainId(1);
        web3Browser.setRpcUrl("https://cerebro.cortexlabs.ai/wallet");
        web3Browser.setWalletAddress(new Address("0x9337d28ae702616abca62f01b7b90fd278bec830"));
        web3Browser.loadUrl("https://digitalclash
