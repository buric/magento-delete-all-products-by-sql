Magento - delete all products by SQL
==================================

Here is the SQL code to delete all products in Magento in a second. 
You don’t have to delete the products through Magento admin. 
Use this in your Magento development system.

```sql
SET FOREIGN_KEY_CHECKS = 0;
TRUNCATE TABLE `catalog_product_bundle_option`;
TRUNCATE TABLE `catalog_product_bundle_option_value`;
TRUNCATE TABLE `catalog_product_bundle_selection`;
TRUNCATE TABLE `catalog_product_entity_datetime`;
TRUNCATE TABLE `catalog_product_entity_decimal`;
TRUNCATE TABLE `catalog_product_entity_gallery`;
TRUNCATE TABLE `catalog_product_entity_int`;
TRUNCATE TABLE `catalog_product_entity_media_gallery`;
TRUNCATE TABLE `catalog_product_entity_media_gallery_value`;
TRUNCATE TABLE `catalog_product_entity_text`;
TRUNCATE TABLE `catalog_product_entity_tier_price`;
TRUNCATE TABLE `catalog_product_entity_varchar`;
TRUNCATE TABLE `catalog_product_link`;
TRUNCATE TABLE `catalog_product_link_attribute`;
TRUNCATE TABLE `catalog_product_link_attribute_decimal`;
TRUNCATE TABLE `catalog_product_link_attribute_int`;
TRUNCATE TABLE `catalog_product_link_attribute_varchar`;
TRUNCATE TABLE `catalog_product_link_type`;
TRUNCATE TABLE `catalog_product_option`;
TRUNCATE TABLE `catalog_product_option_price`;
TRUNCATE TABLE `catalog_product_option_title`;
TRUNCATE TABLE `catalog_product_option_type_price`;
TRUNCATE TABLE `catalog_product_option_type_title`;
TRUNCATE TABLE `catalog_product_option_type_value`;
TRUNCATE TABLE `catalog_product_super_attribute`;
TRUNCATE TABLE `catalog_product_super_attribute_label`;
TRUNCATE TABLE `catalog_product_super_attribute_pricing`;
TRUNCATE TABLE `catalog_product_super_link`;
TRUNCATE TABLE `catalog_product_enabled_index`;
TRUNCATE TABLE `catalog_product_website`;
TRUNCATE TABLE `catalog_product_entity`;
TRUNCATE TABLE `cataloginventory_stock`;
TRUNCATE TABLE `cataloginventory_stock_item`;
TRUNCATE TABLE `cataloginventory_stock_status`;
INSERT INTO `catalog_product_link_type` VALUES(1, 'relation');
INSERT INTO `catalog_product_link_type` VALUES(3, 'super');
INSERT INTO `catalog_product_link_type` VALUES(4, 'up_sell');
INSERT INTO `catalog_product_link_type` VALUES(5, 'cross_sell');
INSERT INTO `catalog_product_link_attribute` VALUES(1, 1, 'position', 'int');
INSERT INTO `catalog_product_link_attribute` VALUES(2, 3, 'position', 'int');
INSERT INTO `catalog_product_link_attribute` VALUES(3, 3, 'qty', 'decimal');
INSERT INTO `catalog_product_link_attribute` VALUES(4, 4, 'position', 'int');
INSERT INTO `catalog_product_link_attribute` VALUES(5, 5, 'position', 'int');
INSERT INTO `cataloginventory_stock` VALUES(1, 'Default');
SET FOREIGN_KEY_CHECKS = 1;
```
