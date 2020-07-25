# Notifier

Trigger different things on receiving a 'walletnotify' from a Zcash or Ycash node based on the receiving address.

This allows you to use the same node for different funtions, and since shielded addresses are private there's no issue in re-using them.

This ONLY works for sheilded addresses (zs1, ys1) 

To use this, edit zcashd.conf (or ycashd.conf) and add the following line :-

walletnotify="/path/to/this/script %s"

