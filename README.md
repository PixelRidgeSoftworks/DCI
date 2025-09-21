# DynamicCursesInput

[![Join our Discord](https://img.shields.io/badge/Discord-Join%20Server-7289DA?logo=discord\&logoColor=white)](https://discord.gg/j6v99ZPkrQ)

DynamicCursesInput is a Ruby gem that simplifies the implementation of dynamic typing in terminal-based user interfaces (TUIs) built with the Curses library. It provides an intuitive way to handle user input, including special keys, without the need for extensive custom code.

---

## 📦 Installation

To install the gem, add it to your Gemfile:

```ruby
gem 'dynamic_curses_input'
```

Then, run:

```bash
bundle install
```

Alternatively, you can install it directly:

```bash
gem install dynamic_curses_input
```

---

## 🚀 Usage Example

Here's a simple example of how to use DynamicCursesInput in your Ruby application:

```ruby
require 'curses'
require 'dynamic_curses_input'

Curses.init_screen
Curses.curs_set(1)

input = DCI.catch_input(true)
puts "You entered: #{input}"

Curses.close_screen
```

In this example, `DCI.catch_input(true)` captures user input, allowing for dynamic editing and special key handling.

---

## 🛠️ Dependencies

DynamicCursesInput requires the following gems:

* `curses` (\~> 1.4)
* `reline` (\~> 0.3.8)

It also has a development dependency on:

* `rubocop` (\~> 1.56)

---

## 📄 License

This gem is licensed under the PixelRidge-BEGPULSE license.

---

## 📞 Support

For support or inquiries, please join our Discord community:

[![Join our Discord](https://img.shields.io/badge/Discord-Join%20Server-7289DA?logo=discord\&logoColor=white)](https://discord.gg/j6v99ZPkrQ)

---

## ⚠️ Known Issues

* **X & Y Coordinates for Window Placement**: There is a known bug where the X and Y coordinates for placing windows may not function correctly. This issue will be addressed in the next update. In the meantime, it's recommended to use the preset window locations.

---

## 🧪 Development

To contribute or run tests locally, clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/PixelRidgeSoftworks/DCI.git
cd DCI
bundle install
```

Run tests using:

```bash
bundle exec rspec
```

Run RuboCop for linting:

```bash
bundle exec rubocop
```

---

## 🔗 Links

* [Gem on RubyGems](https://rubygems.org/gems/dynamic_curses_input)
* [Source Code on GitHub](https://github.com/PixelRidgeSoftworks/DCI)

---
