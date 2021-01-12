## Try it out

1.  It's dangerous to go alone.  Take this!  https://www.rustup.rs/

2.  Use the stable rust compiler.

```sh
rustup install stable
rustup default stable

```

2.  Fetch the plugin.

```sh
$ git clone https://github.com/hardliner66/neovim-twitch-chat
```

3.  Build the binary portion of the plugin.

```sh
$ cd neovim-twitch-chat
$ cargo build --release
```

4.  Test it out in a fresh instance of Neovim. *(If Windows requires any
    changes, open an issue!)*

```sh
nvim -u ./init.vim --noplugin -c ":TwitchChatConnect"
```

The `TwitchChatConnect` command spawns the Rust plugin in a separate process and
establishes a channel.

