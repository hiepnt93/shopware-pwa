## API Report File for "@shopware-pwa/helpers"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { CmsPage } from '@shopware-pwa/shopware-6-client/src/interfaces/models/content/cms/CmsPage';
import { CmsSection } from '@shopware-pwa/shopware-6-client/src/interfaces/models/content/cms/CmsPage';
import { Product } from '@shopware-pwa/shopware-6-client/src/interfaces/models/content/product/Product';
import { PropertyGroupOption } from '@shopware-pwa/shopware-6-client/src/interfaces/models/content/property/PropertyGroupOption';
import { SearchCriteria } from '@shopware-pwa/shopware-6-client/src/interfaces/search/SearchCriteria';
import { Sort } from '@shopware-pwa/shopware-6-client/src/interfaces/search/SearchCriteria';
import { UiMediaGalleryItem as UiMediaGalleryItem_2 } from '@shopware-pwa/helpers';
import { UiProductOption as UiProductOption_2 } from '@shopware-pwa/helpers';
import { UiProductProperty as UiProductProperty_2 } from '@shopware-pwa/helpers';
import { UiProductReview as UiProductReview_2 } from '@shopware-pwa/helpers';

// @alpha (undocumented)
export interface CategoryFilterEntityValue {
    // (undocumented)
    customFields: any;
    // (undocumented)
    description: string | null;
    // (undocumented)
    name: string;
}

// @alpha (undocumented)
export interface CategoryFilterEntityValues {
    // (undocumented)
    [valueId: string]: CategoryFilterEntityValue;
}

// @alpha (undocumented)
export interface CategoryFilterRangeValues {
    // (undocumented)
    max: string;
    // (undocumented)
    min: string;
}

// @alpha (undocumented)
export interface CategoryFilterTermValue {
    // (undocumented)
    count: number;
    // (undocumented)
    extensions: any;
    // (undocumented)
    key: string;
}

// @alpha (undocumented)
export function exportUrlQuery(searchCriteria: SearchCriteria): string | undefined;

// @alpha (undocumented)
export function getCategoryAvailableFilters({ filters }?: {
    filters?: Filter;
}): UiCategoryFilter[];

// @alpha (undocumented)
export function getCategoryAvailableSorting({ sorting }?: {
    sorting?: Sorting;
}): UiCategorySorting[];

// @alpha (undocumented)
export function getCmsSections(content: CmsPage): CmsSection[];

// @alpha (undocumented)
export const getFilterSearchCriteria: (selectedFilters: any) => any[];

// @alpha (undocumented)
export function getProductMainImageUrl({ product }?: {
    product?: Product;
}): string;

// @alpha (undocumented)
export function getProductMediaGallery({ product }?: {
    product?: Product;
}): UiMediaGalleryItem_2[];

// @alpha (undocumented)
export function getProductName({ product }?: {
    product?: Product;
}): string | null;

// @alpha (undocumented)
export function getProductOption({ product, attribute }?: {
    product?: Product;
    attribute?: string;
}): PropertyGroupOption | undefined;

// Warning: (ae-forgotten-export) The symbol "ProductOptions" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export function getProductOptions({ product }?: {
    product?: Product;
}): ProductOptions;

// @alpha (undocumented)
export function getProductOptionsUrl({ product, options }?: {
    product?: Product;
    options?: string[];
}): string;

// @alpha (undocumented)
export function getProductProperties({ product }?: {
    product?: Product;
}): UiProductProperty_2[];

// @alpha (undocumented)
export function getProductRegularPrice({ product }?: {
    product?: Product;
}): number;

// @alpha (undocumented)
export function getProductReviews({ product }?: {
    product?: Product;
}): UiProductReview_2[];

// @alpha (undocumented)
export function getProductSpecialPrice(product: Product): number;

// @alpha (undocumented)
export function getProductUrl(product: Product | null): string;

// @alpha (undocumented)
export const getSortingLabel: (sorting: SwSorting) => string;

// @alpha (undocumented)
export const getSortingSearchCriteria: (selectedSorting: SwSorting) => Sort;

// @alpha (undocumented)
export function getVariantOptionsLabel({ product }?: {
    product?: Product;
}): string | null;

// @alpha (undocumented)
export function isProductSimple({ product }?: {
    product?: Product;
}): boolean;

// @alpha (undocumented)
export function parseUrlQuery(query: any): SearchCriteria;

// @alpha (undocumented)
export interface SwSorting {
    // (undocumented)
    active: boolean;
    // (undocumented)
    field: string;
    // (undocumented)
    name: string;
    // (undocumented)
    order: string;
}

// @alpha (undocumented)
export interface UiCategoryFilter {
    // (undocumented)
    name: string;
    // Warning: (ae-forgotten-export) The symbol "UiCategoryFilterOption" needs to be exported by the entry point index.d.ts
    // Warning: (ae-forgotten-export) The symbol "UiCategoryRangeFilterOption" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    options: UiCategoryFilterOption[] | UiCategoryRangeFilterOption | any;
    // (undocumented)
    type: UiCategoryFilterType;
}

// @public (undocumented)
export enum UiCategoryFilterType {
    // (undocumented)
    entity = "entity",
    // (undocumented)
    max = "max",
    // (undocumented)
    range = "range",
    // (undocumented)
    term = "term"
}

// @alpha (undocumented)
export interface UiCategorySorting {
    // (undocumented)
    active: boolean;
    // (undocumented)
    field: string;
    // (undocumented)
    name: string;
    // (undocumented)
    order: string;
}

// @alpha (undocumented)
export interface UiMediaGalleryItem {
    // (undocumented)
    big: UiMediaGalleryItemUrl;
    // (undocumented)
    normal: UiMediaGalleryItemUrl;
    // (undocumented)
    small: UiMediaGalleryItemUrl;
}

// @alpha (undocumented)
export interface UiMediaGalleryItemUrl {
    // (undocumented)
    url: string;
}

// @alpha (undocumented)
export interface UiProductOption {
    // (undocumented)
    [attribute: string]: string;
    // (undocumented)
    attribute: string;
    // (undocumented)
    code: string;
    // (undocumented)
    label: string;
    // (undocumented)
    value: string;
}

// @alpha (undocumented)
export interface UiProductProperty {
    // (undocumented)
    name: string;
    // (undocumented)
    value: string | null;
}

// @alpha (undocumented)
export interface UiProductReview {
    // (undocumented)
    author: string;
    // (undocumented)
    date: Date;
    // (undocumented)
    id: string;
    // (undocumented)
    message: string | null;
    // (undocumented)
    rating: number | null;
}


// Warnings were encountered during analysis:
//
// dist/packages/helpers/src/category/getCategoryAvailableFilters.d.ts:42:5 - (ae-forgotten-export) The symbol "Filter" needs to be exported by the entry point index.d.ts
// dist/packages/helpers/src/category/getCategoryAvailableSorting.d.ts:12:5 - (ae-forgotten-export) The symbol "Sorting" needs to be exported by the entry point index.d.ts

// (No @packageDocumentation comment for this package)

```