<script>
	let faqInfos = [
		{
			header: 'How to Connect a crypto wallet',
			body: 'A Metamask wallet is required for the storage of cryptocurrency and for the storage of your Martian NFT. Download Metamask and add the extension to your browser. Once you are on our website, press the “Connect Wallet" button located in the Metamask extension. For more information on how to set up your Metamask wallet, please visit https://metamask.io/.'
		},
		{
			header: 'Buying the correct amount of ETH.',
			body: 'ETH is the currency used on the Ethereum blockchain network. You can purchase ETH using your Metamask wallet. Once in your wallet, press the “buy” button and use either Wyre or Transak to purchase your ETH. We recommend purchasing a little extra so that you have enough to cover gas fees.'
		},
		{
			header: 'What are gas fees?',
			body: 'Just as it takes gas to power a car, it takes computing power to maintain the blockchain and deploy/execute the smart contracts that signify these images as non-fungible ERC-721 tokens. To see what the gas prices are now, check the Ethereum Gas Tracker on our server. Gas fees are displayed in the unit, Gwei.\n\nGwei is a term for a very small amount of the Ethereum cryptocurrency and is commonly used when discussing transaction fees on the Ethereum network. One Gwei is equal to 0.000000001 ETH. If a transaction cost is 0.000000020 ETH, you would say that the cost was 20 Gwei.'
		},
		{
			header: 'How to mint your Martian',
			body: 'The process of purchasing your Martian and having it verified as an NFT on the blockchain is called minting. Once your wallet is connected, navigate to the Mint section of our website. It is important that your wallet is connected to the Ethereum Mainnet network before minting.'
		},
		{
			header: "Where can I find my Martian?",
			body: 'Once minted, your Martian will be transferred to your Metamask wallet. It may take a little time for the NFT to show up on Metamask, it can be found under the ”NFT” section on the app. We recommend that you also connect your wallet to OpenSea. https://opensea.io/  \n\nYour Martian will also be viewable on OpenSea in your “collected” section. You can use this to import the NFT to a MetaMask wallet. Navigate to “import NFT” within your MetaMask mobile app (make sure you are on the wallet account you minted from). Then input the contract address and token ID found in the details section of your NFT, viewable in OpenSea.'
		}
	];
</script>

<section id="faq" class="h-full place-content-center text-white my-32">
	<h1 class="text-6xl text-primary font-black my-8"><span class="text-shadow">FAQ</span></h1>
	{#each faqInfos as faqInfo}
		<article class="my-5">
			<h3 class="text-secondary text-xl font-black">{faqInfo.header}</h3>
			<pre class="mt-5 px-7 whitespace-pre-wrap text-md sm:text-lg font-['Inconsolata']">{faqInfo.body}</pre>
		</article>
	{/each}
</section>

<style>
	.text-shadow {
		text-shadow: 1px 0 20px rgb(200 255 0 / 31%);
	}
</style>
