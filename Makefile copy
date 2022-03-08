build:
	cd nft && daml build
	cd nft && codegen js -o daml.js .daml/dist/nft-0.0.1.dar

deploy: build
	mkdir -p deploy
	cp nft/.daml/dist/*.dar deploy

clean:
	cd nft && rm -rf .daml
	cd nft && rm -rf daml.js
	rm -rf deploy
