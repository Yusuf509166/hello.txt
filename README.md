class HelloBabu {
    constructor(runtime) {
        this.runtime = runtime;
    }

    getInfo() {
        return {
            id: 'helloBabu',
            name: 'Hello Babu!',
            blocks: [
                {
                    opcode: 'sayHelloBabu',
                    blockType: this.BlockType.VOID,
                    text: 'Say "Hello Babu!"',
                    func: 'sayHelloBabu'
                },
            ]
        };
    }

    sayHelloBabu() {
        console.log('Hello Babu!');
    }
}

Scratch.extensions.register('Hello Babu', new HelloBabu());
