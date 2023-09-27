# Changelog

## [2023-09-27]

### Added

Introduced `accepted` status for Orders. This status denotes that the order has been
accepted by the seller and processing has started. Primary use is to provide a distinction
between new unseen orders and unacknowledged but seen orders.

### Changed

The `order_date` field for the Order payload is now the creation date of the order instead of the 
original e-commerce order date. An order can be a reorder due to a cancellation or replacement, new
orders can exist with an original order date days or weeks in the past.
