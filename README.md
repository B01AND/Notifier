# Notifier

Triggers different things on receiving a 'walletnotify' from a Zcash or Ycash node based on the receiving address.

This allows you to use the same node for different funtions, and as shielded addresses are private there's no issue in re-using them.

This ONLY works for sheilded addresses (zs1, ys1) 

To use this, edit zcashd.conf (or ycashd.conf) and add the following line :-

walletnotify="/path/to/this/script %s"

In the walletnotify.conf file :-

  %txid   - transaction ID
  %zaddr  - shielded address involved in this transaction

You can also specify a default action for each coin type if the sheilded address is not specified.
