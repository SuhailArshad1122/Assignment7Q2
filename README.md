// following is main.rs
mod lib;
fn main () {
    lib::mod_in_lib1::mod_in_lib2::simple_fn()
}

// following is lib.rs
pub mod mod_in_lib1 {
    pub mod mod_in_lib2 {
        pub fn simple_fn() {
            println!("Simple Function in sub module from lib");
        }
    }
}
