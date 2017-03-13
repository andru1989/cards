# Cards

### How to use

Open an interactive elixir console with `iex -S mix` then:

  - Step by step do the following:

    ```elixir
    iex> deck = Cards.create_deck
    iex> deck = Cards.shuffle(deck)
    iex> {hand, deck} = Cards.deal(deck, 1)
    iex> hand # Then you have your hand cards

    ```

  - You can also use the pipe operator with just one line:

    ```elixir
    iex> {hand, deck} = Cards.create_deck |> Cards.shuffle |> Cards.deal(2)
    iex> hand # Then you have your hand cards
    ```
