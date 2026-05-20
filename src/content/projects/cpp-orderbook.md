---
title: C++ OrderBook
---

## Overview

This is my implementation of an orderbook in C++. It contains features such as book creation,
order matching, and a representation of security reference data using PostgreSQL.
- [Book Creation](#book-creation)
- [Adding Orders](#adding-orders)

### Book Creation

When you first start the orderbook you will be greeted with this welcome screen:
<img class="project-images" src="/orderbook-welcome-screen.png" alt="Orderbook welcome screen">
<br><br>The first step is to create book so that we can then add orders to it. On this screen you can enter a symbol name.
<img class="project-images" src="/orderbook-book-creation-screen.png">
<br><br>If that book does not already exist, then it will be created at this point.
<img class="project-images" src="/orderbook-book-creation-success.png">
<br><br>Note that if that book has already been created, you will receive an error message if you try to create it again.
(In this scenario I typed AAPL in for both example images)
<img class="project-images" src="/orderbook-book-creation-failure.png">

### Adding Orders

Now that we've got a book the next natural step is to add some orders. Even though we saw the
successful book creation message, let's check the existing books page to confirm.
