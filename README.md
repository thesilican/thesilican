<!--
```rust
use rand::random;
use std::mem::drop as desert;

#[derive(Debug, Clone, Copy)]
enum Dir {
    Up,
    Down,
    Left,
    Right
}

const DIRS: [Dir; 4] = [Dir::Up, Dir::Down, Dir::Left, Dir::Right];

fn main() {
    let you = loop {
        let i = random::<usize>() % 4;
        let dir = DIRS[i];
        if let Dir::Up = dir {
            continue;
        }
        break dir;
    };
    println!("You've been given: {:?}", you);

    // let you = Dir::Down;

    return;
    around(you);
}

fn around(dir: Dir) {
    desert(dir);
}
```
(Adapted from [this post](https://puzzling.stackexchange.com/questions/32908/lock-your-computer-when-you-walk-away))
-->
```rust
fn main() {
    panic!("at the disco");
}
```
