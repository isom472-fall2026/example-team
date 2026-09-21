# Proposal — Northgate Bakery order book

*This is the worked example for ISOM 472. The team and the client are invented. Read it for
the shape and the level of detail, then write your own about your own client.*

## 1. The client, and how you reach them

Northgate Bakery, a single shop in Salmiya with four staff. Our contact is Fajer Al-Otaibi,
who owns it and works the counter most mornings. Two of us buy bread there; we met her on
14 September and she has agreed to a fifteen-minute call every second Sunday.

## 2. What happens today, and what goes wrong

Orders for cakes and large bread trays arrive on the shop's WhatsApp. Whoever has the phone
writes the order in a paper notebook by the till. At the end of the day the notebook is not
copied anywhere. When the morning person is off, the evening person cannot tell which orders
were already baked. Fajer says about four orders a week are either baked twice or missed
entirely, and the missed ones are found out when the customer arrives.

## 3. Who is better off, and how you would know

The counter staff, who would stop guessing, and the customer who arrives to collect. The
signal is the number of orders baked twice or missed in a week. Fajer counts it now from
memory; she agreed to write the number down each week from 21 September, so we have a
before and an after.

## 4. What the system does, in outline

- Record an order: customer name, phone, what was ordered, the day it is wanted
- Show today's orders, in the order they are wanted
- Mark an order as baked, and mark it as collected
- Flag two orders that look like the same order — same customer, same day
- Show last week's orders so nothing has to be remembered

## 5. What it records

| Thing | What it holds |
|---|---|
| Customer | name, phone |
| Order | which customer, what was ordered, day wanted, state (new · baked · collected) |
| Staff member | who marked an order baked or collected |

One customer has many orders. Every change of state records who made it.

## 6. In scope by the final week — and what is not

**Working by the final week:** recording an order, the day's list, marking baked and
collected, the duplicate flag, and last week's list. Staff sign in with an email and
password.

**Deliberately not:** payments, delivery, stock or ingredients, the Instagram orders Fajer
also gets, and anything on the customer's phone. WhatsApp itself is untouched — orders are
still read there and typed in here.

## 7. After the semester

Fajer can keep using it on the shop's tablet; it costs nothing to run at her volume. The
code stays public, so the next team, or the next student she hires, can pick it up. If she
outgrows it, what she has is a written description of exactly what her shop needs, which is
worth more to a supplier than a conversation.

## 8. What you told the client this is

We told Fajer on 14 September that this is a student project for a university course, built
by four students over one semester; that the code and the page are public and anyone can
read them; that we will not put her customers' real phone numbers in it while we build; and
that after the final week in December nobody is paid to fix it, though she may keep using
it. She said that was fine and asked for it to be "simple enough for Mariam", her evening
counter staff.
