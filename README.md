# anarchy-kotlin
## Anything is possible

For a quick start, paste the following at the top of any kotlin file:

```
@file:Suppress("UNSUPPORTED", "UNSUPPORTED_WARNING", "NEW_INFERENCE_ERROR", "NEW_INFERENCE_DIAGNOSTIC", "NON_APPLICABLE_CALL_FOR_BUILDER_INFERENCE", "UNSUPPORTED_FEATURE", "EXCEPTION_FROM_ANALYZER", "MISSING_STDLIB", "EXPERIMENTAL_FEATURE_WARNING", "EXPERIMENTAL_FEATURE_ERROR", "EXPLICIT_BACKING_FIELDS_UNSUPPORTED", "REDECLARATION", "PACKAGE_OR_CLASSIFIER_REDECLARATION", "DUPLICATE_PARAMETER_NAME_IN_FUNCTION_TYPE", "EXTENSION_SHADOWED_BY_MEMBER", "EXTENSION_FUNCTION_SHADOWED_BY_INNER_CLASS_CONSTRUCTOR", "EXTENSION_FUNCTION_SHADOWED_BY_MEMBER_PROPERTY_WITH_INVOKE", "UNRESOLVED_REFERENCE", "DEPRECATION", "DEPRECATION_ERROR", "TYPEALIAS_EXPANSION_DEPRECATION", "TYPEALIAS_EXPANSION_DEPRECATION_ERROR", "VERSION_REQUIREMENT_DEPRECATION", "VERSION_REQUIREMENT_DEPRECATION_ERROR", "OVERRIDE_DEPRECATION", "DEPRECATED_SINCE_KOTLIN_WITHOUT_DEPRECATED", "DEPRECATED_SINCE_KOTLIN_WITH_DEPRECATED_LEVEL", "DEPRECATED_SINCE_KOTLIN_WITH_UNORDERED_VERSIONS", "DEPRECATED_SINCE_KOTLIN_WITHOUT_ARGUMENTS", "DEPRECATED_SINCE_KOTLIN_OUTSIDE_KOTLIN_SUBPACKAGE", "API_NOT_AVAILABLE", "MISSING_DEPENDENCY_CLASS", "MISSING_DEPENDENCY_SUPERCLASS", "MISSING_BUILT_IN_DECLARATION", "MISSING_SCRIPT_BASE_CLASS", "MISSING_SCRIPT_STANDARD_TEMPLATE", "MISSING_SCRIPT_RECEIVER_CLASS", "MISSING_IMPORTED_SCRIPT_FILE", "MISSING_IMPORTED_SCRIPT_PSI", "MISSING_SCRIPT_PROVIDED_PROPERTY_CLASS", "PRE_RELEASE_CLASS", "IR_WITH_UNSTABLE_ABI_COMPILED_CLASS", "FIR_COMPILED_CLASS", "INCOMPATIBLE_CLASS", "INVISIBLE_REFERENCE", "INVISIBLE_MEMBER", "DEPRECATED_ACCESS_BY_SHORT_NAME", "DEPRECATED_ACCESS_TO_ENUM_COMPANION_PROPERTY", "DEPRECATED_RESOLVE_WITH_AMBIGUOUS_ENUM_ENTRY", "PROTECTED_CONSTRUCTOR_NOT_IN_SUPER_CALL", "EXPOSED_PROPERTY_TYPE", "EXPOSED_FUNCTION_RETURN_TYPE", "EXPOSED_PARAMETER_TYPE", "EXPOSED_RECEIVER_TYPE", "EXPOSED_TYPE_PARAMETER_BOUND", "EXPOSED_SUPER_CLASS", "EXPOSED_SUPER_INTERFACE", "EXPOSED_TYPEALIAS_EXPANDED_TYPE", "EXPOSED_FROM_PRIVATE_IN_FILE", "INACCESSIBLE_TYPE", "PLATFORM_CLASS_MAPPED_TO_KOTLIN", "PROJECTION_ON_NON_CLASS_TYPE_ARGUMENT", "UPPER_BOUND_VIOLATED", "UPPER_BOUND_VIOLATED_WARNING", "REDUNDANT_NULLABLE", "NULLABLE_ON_DEFINITELY_NOT_NULLABLE", "INCORRECT_LEFT_COMPONENT_OF_INTERSECTION", "INCORRECT_RIGHT_COMPONENT_OF_INTERSECTION", "WRONG_NUMBER_OF_TYPE_ARGUMENTS", "OUTER_CLASS_ARGUMENTS_REQUIRED", "TYPE_ARGUMENTS_NOT_ALLOWED", "NO_TYPE_ARGUMENTS_ON_RHS", "CONFLICTING_PROJECTION", "REDUNDANT_PROJECTION", "TYPE_VARIANCE_CONFLICT_IN_EXPANDED_TYPE", "FINITE_BOUNDS_VIOLATION", "FINITE_BOUNDS_VIOLATION_IN_JAVA", "EXPANSIVE_INHERITANCE", "EXPANSIVE_INHERITANCE_IN_JAVA", "TYPE_ARGUMENTS_FOR_OUTER_CLASS_WHEN_NESTED_REFERENCED", "REIFIED_TYPE_IN_CATCH_CLAUSE", "TYPE_PARAMETER_IN_CATCH_CLAUSE", "GENERIC_THROWABLE_SUBCLASS", "INNER_CLASS_OF_GENERIC_THROWABLE_SUBCLASS", "INNER_CLASS_OF_GENERIC_THROWABLE_SUBCLASS_WARNING", "TOPLEVEL_TYPEALIASES_ONLY", "RECURSIVE_TYPEALIAS_EXPANSION", "UPPER_BOUND_VIOLATED_IN_TYPEALIAS_EXPANSION", "UPPER_BOUND_VIOLATED_IN_TYPEALIAS_EXPANSION_WARNING", "CONFLICTING_PROJECTION_IN_TYPEALIAS_EXPANSION", "TYPEALIAS_SHOULD_EXPAND_TO_CLASS", "TYPEALIAS_EXPANDED_TO_MALFORMED_TYPE", "EXPANDED_TYPE_CANNOT_BE_CONSTRUCTED", "EXPANDED_TYPE_CANNOT_BE_INHERITED", "DEPRECATED_SYNTAX_WITH_DEFINITELY_NOT_NULL", "MODIFIER_LIST_NOT_ALLOWED", "CANNOT_ALL_UNDER_IMPORT_FROM_SINGLETON", "CANNOT_BE_IMPORTED", "PACKAGE_CANNOT_BE_IMPORTED", "CONFLICTING_IMPORT", "OPERATOR_RENAMED_ON_IMPORT", "INCOMPATIBLE_MODIFIERS", "DEPRECATED_MODIFIER_PAIR", "REPEATED_MODIFIER", "REDUNDANT_MODIFIER", "WRONG_MODIFIER_TARGET", "DEPRECATED_MODIFIER_FOR_TARGET", "DEPRECATED_MODIFIER", "REDUNDANT_MODIFIER_FOR_TARGET", "NO_EXPLICIT_VISIBILITY_IN_API_MODE", "NO_EXPLICIT_RETURN_TYPE_IN_API_MODE", "NO_EXPLICIT_VISIBILITY_IN_API_MODE_WARNING", "NO_EXPLICIT_RETURN_TYPE_IN_API_MODE_WARNING", "WRONG_MODIFIER_CONTAINING_DECLARATION", "DEPRECATED_MODIFIER_CONTAINING_DECLARATION", "ILLEGAL_INLINE_PARAMETER_MODIFIER", "INLINE_SUSPEND_FUNCTION_TYPE_UNSUPPORTED", "REDUNDANT_INLINE_SUSPEND_FUNCTION_TYPE", "WRONG_ANNOTATION_TARGET", "WRONG_ANNOTATION_TARGET_WITH_USE_SITE_TARGET", "WRONG_ANNOTATION_TARGET_WITH_USE_SITE_TARGET_ON_TYPE", "REPEATED_ANNOTATION", "REPEATED_ANNOTATION_WARNING", "NON_SOURCE_ANNOTATION_ON_INLINED_LAMBDA_EXPRESSION", "WRONG_EXTENSION_FUNCTION_TYPE", "WRONG_EXTENSION_FUNCTION_TYPE_WARNING", "SUPERTYPES_FOR_ANNOTATION_CLASS", "MISSING_VAL_ON_ANNOTATION_PARAMETER", "VAR_ANNOTATION_PARAMETER", "ANNOTATION_CLASS_CONSTRUCTOR_CALL", "NOT_AN_ANNOTATION_CLASS", "ANNOTATION_CLASS_MEMBER", "INVALID_TYPE_OF_ANNOTATION_MEMBER", "NULLABLE_TYPE_OF_ANNOTATION_MEMBER", "ANNOTATION_ARGUMENT_MUST_BE_CONST", "ANNOTATION_ARGUMENT_MUST_BE_KCLASS_LITERAL", "ANNOTATION_ARGUMENT_MUST_BE_ENUM_CONST", "ANNOTATION_ARGUMENT_KCLASS_LITERAL_OF_TYPE_PARAMETER", "ANNOTATION_ARGUMENT_KCLASS_LITERAL_OF_TYPE_PARAMETER_ERROR", "ANNOTATION_PARAMETER_DEFAULT_VALUE_MUST_BE_CONSTANT", "ANNOTATIONS_ON_BLOCK_LEVEL_EXPRESSION_ON_THE_SAME_LINE", "ANNOTATION_USED_AS_ANNOTATION_ARGUMENT", "ANNOTATION_ARGUMENT_IS_NON_CONST", "ILLEGAL_KOTLIN_VERSION_STRING_VALUE", "NEWER_VERSION_IN_SINCE_KOTLIN", "OPT_IN_USAGE", "OPT_IN_USAGE_ERROR", "OPT_IN_USAGE_FUTURE_ERROR", "OPT_IN_OVERRIDE", "OPT_IN_OVERRIDE_ERROR", "OPT_IN_IS_NOT_ENABLED", "OPT_IN_CAN_ONLY_BE_USED_AS_ANNOTATION", "OPT_IN_MARKER_CAN_ONLY_BE_USED_AS_ANNOTATION_OR_ARGUMENT_IN_OPT_IN", "OPT_IN_WITHOUT_ARGUMENTS", "OPT_IN_ARGUMENT_IS_NOT_MARKER", "OPT_IN_MARKER_WITH_WRONG_TARGET", "OPT_IN_MARKER_WITH_WRONG_RETENTION", "OPT_IN_MARKER_ON_WRONG_TARGET", "OPT_IN_MARKER_ON_OVERRIDE", "OPT_IN_MARKER_ON_OVERRIDE_WARNING", "SUBCLASS_OPT_IN_INAPPLICABLE", "EXPERIMENTAL_UNSIGNED_LITERALS", "EXPERIMENTAL_UNSIGNED_LITERALS_ERROR", "NON_PARENTHESIZED_ANNOTATIONS_ON_FUNCTIONAL_TYPES", "ANNOTATION_IN_WHERE_CLAUSE_WARNING", "CONST_VAL_NOT_TOP_LEVEL_OR_OBJECT", "CONST_VAL_WITH_GETTER", "CONST_VAL_WITH_DELEGATE", "TYPE_CANT_BE_USED_FOR_CONST_VAL", "CONST_VAL_WITHOUT_INITIALIZER", "CONST_VAL_WITH_NON_CONST_INITIALIZER", "NON_CONST_VAL_USED_IN_CONSTANT_EXPRESSION", "INAPPLICABLE_TARGET_ON_PROPERTY", "INAPPLICABLE_TARGET_PROPERTY_IMMUTABLE", "INAPPLICABLE_TARGET_PROPERTY_HAS_NO_DELEGATE", "INAPPLICABLE_TARGET_PROPERTY_HAS_NO_BACKING_FIELD", "INAPPLICABLE_PARAM_TARGET", "REDUNDANT_ANNOTATION_TARGET", "INAPPLICABLE_FILE_TARGET", "PROJECTION_IN_IMMEDIATE_ARGUMENT_TO_SUPERTYPE", "CYCLIC_INHERITANCE_HIERARCHY", "CYCLIC_SCOPES_WITH_COMPANION", "SUPERTYPE_NOT_INITIALIZED", "DELEGATION_NOT_TO_INTERFACE", "DELEGATED_MEMBER_HIDES_SUPERTYPE_OVERRIDE", "SUPERTYPE_NOT_A_CLASS_OR_INTERFACE", "SUPERTYPE_IS_EXTENSION_FUNCTION_TYPE", "SUPERTYPE_IS_SUSPEND_FUNCTION_TYPE", "SUPERTYPE_IS_KSUSPEND_FUNCTION_TYPE", "MIXING_SUSPEND_AND_NON_SUSPEND_SUPERTYPES", "MANY_CLASSES_IN_SUPERTYPE_LIST", "SUPERTYPE_APPEARS_TWICE", "INCONSISTENT_TYPE_PARAMETER_VALUES", "INCONSISTENT_TYPE_PARAMETER_BOUNDS", "FINAL_SUPERTYPE", "DATA_CLASS_CANNOT_HAVE_CLASS_SUPERTYPES", "SINGLETON_IN_SUPERTYPE", "NULLABLE_SUPERTYPE", "DYNAMIC_SUPERTYPE", "CLASS_CANNOT_BE_EXTENDED_DIRECTLY", "MISSING_CONSTRUCTOR_KEYWORD", "MISSING_CONSTRUCTOR_BRACKETS", "NON_PRIVATE_CONSTRUCTOR_IN_ENUM", "NON_PRIVATE_CONSTRUCTOR_IN_SEALED", "NON_PRIVATE_OR_PROTECTED_CONSTRUCTOR_IN_SEALED", "VALUE_CLASS_NOT_TOP_LEVEL", "VALUE_CLASS_NOT_FINAL", "ABSENCE_OF_PRIMARY_CONSTRUCTOR_FOR_VALUE_CLASS", "INLINE_CLASS_CONSTRUCTOR_WRONG_PARAMETERS_SIZE", "VALUE_CLASS_EMPTY_CONSTRUCTOR", "VALUE_CLASS_CONSTRUCTOR_NOT_FINAL_READ_ONLY_PARAMETER", "PROPERTY_WITH_BACKING_FIELD_INSIDE_VALUE_CLASS", "DELEGATED_PROPERTY_INSIDE_VALUE_CLASS", "VALUE_CLASS_HAS_INAPPLICABLE_PARAMETER_TYPE", "VALUE_CLASS_CANNOT_IMPLEMENT_INTERFACE_BY_DELEGATION", "VALUE_CLASS_CANNOT_EXTEND_CLASSES", "VALUE_CLASS_CANNOT_BE_RECURSIVE", "RESERVED_MEMBER_INSIDE_VALUE_CLASS", "SECONDARY_CONSTRUCTOR_WITH_BODY_INSIDE_VALUE_CLASS", "INNER_CLASS_INSIDE_VALUE_CLASS", "VALUE_CLASS_CANNOT_BE_CLONEABLE", "INLINE_CLASS_DEPRECATED", "INLINE_CLASS_CANNOT_HAVE_CONTEXT_RECEIVERS", "INEFFICIENT_EQUALS_OVERRIDING_IN_INLINE_CLASS", "RESULT_CLASS_IN_RETURN_TYPE", "RESULT_CLASS_WITH_NULLABLE_OPERATOR", "FUN_INTERFACE_WRONG_COUNT_OF_ABSTRACT_MEMBERS", "FUN_INTERFACE_CANNOT_HAVE_ABSTRACT_PROPERTIES", "FUN_INTERFACE_ABSTRACT_METHOD_WITH_TYPE_PARAMETERS", "FUN_INTERFACE_ABSTRACT_METHOD_WITH_DEFAULT_VALUE", "FUN_INTERFACE_CONSTRUCTOR_REFERENCE", "FUN_INTERFACE_WITH_SUSPEND_FUNCTION", "CYCLIC_CONSTRUCTOR_DELEGATION_CALL", "CONSTRUCTOR_IN_OBJECT", "SUPERTYPE_INITIALIZED_WITHOUT_PRIMARY_CONSTRUCTOR", "PRIMARY_CONSTRUCTOR_DELEGATION_CALL_EXPECTED", "PRIMARY_CONSTRUCTOR_DELEGATION_CALL_EXPECTED_IN_ENUM", "DELEGATION_SUPER_CALL_IN_ENUM_CONSTRUCTOR", "PRIMARY_CONSTRUCTOR_REQUIRED_FOR_DATA_CLASS", "EXPLICIT_DELEGATION_CALL_REQUIRED", "INSTANCE_ACCESS_BEFORE_SUPER_CALL", "REDUNDANT_OPEN_IN_INTERFACE", "CONSTRUCTOR_IN_INTERFACE", "METHOD_OF_ANY_IMPLEMENTED_IN_INTERFACE", "SUPERTYPE_INITIALIZED_IN_INTERFACE", "DELEGATION_IN_INTERFACE", "INTERFACE_WITH_SUPERCLASS", "CLASS_IN_SUPERTYPE_FOR_ENUM", "TYPE_PARAMETERS_IN_ENUM", "ENUM_ENTRY_SHOULD_BE_INITIALIZED", "ENUM_CLASS_CONSTRUCTOR_CALL", "SEALED_CLASS_CONSTRUCTOR_CALL", "SEALED_SUPERTYPE", "SEALED_SUPERTYPE_IN_LOCAL_CLASS", "SEALED_INHERITOR_IN_DIFFERENT_PACKAGE", "SEALED_INHERITOR_IN_DIFFERENT_MODULE", "CLASS_INHERITS_JAVA_SEALED_CLASS", "MANY_COMPANION_OBJECTS", "LOCAL_OBJECT_NOT_ALLOWED", "LOCAL_INTERFACE_NOT_ALLOWED", "TYPE_PARAMETERS_IN_OBJECT", "TYPE_PARAMETERS_IN_ANONYMOUS_OBJECT", "FINAL_UPPER_BOUND", "DYNAMIC_UPPER_BOUND", "UPPER_BOUND_IS_EXTENSION_FUNCTION_TYPE", "ONLY_ONE_CLASS_BOUND_ALLOWED", "BOUNDS_NOT_ALLOWED_IF_BOUNDED_BY_TYPE_PARAMETER", "REPEATED_BOUND", "CONFLICTING_UPPER_BOUNDS", "NAME_IN_CONSTRAINT_IS_NOT_A_TYPE_PARAMETER", "VARIANCE_ON_TYPE_PARAMETER_NOT_ALLOWED", "BOUND_ON_TYPE_ALIAS_PARAMETER_NOT_ALLOWED", "DEPRECATED_TYPE_PARAMETER_SYNTAX", "REIFIED_TYPE_PARAMETER_NO_INLINE", "TYPE_PARAMETERS_NOT_ALLOWED", "TYPE_PARAMETER_OF_PROPERTY_NOT_USED_IN_RECEIVER", "CYCLIC_GENERIC_UPPER_BOUND", "MISPLACED_TYPE_PARAMETER_CONSTRAINTS", "CONFLICTING_OVERLOADS", "NON_FINAL_MEMBER_IN_FINAL_CLASS", "NON_FINAL_MEMBER_IN_OBJECT", "NOTHING_TO_OVERRIDE", "VIRTUAL_MEMBER_HIDDEN", "CANNOT_OVERRIDE_INVISIBLE_MEMBER", "DATA_CLASS_OVERRIDE_CONFLICT", "CANNOT_INFER_VISIBILITY", "OVERRIDING_FINAL_MEMBER", "CANNOT_WEAKEN_ACCESS_PRIVILEGE", "CANNOT_CHANGE_ACCESS_PRIVILEGE", "RETURN_TYPE_MISMATCH_ON_OVERRIDE", "PROPERTY_TYPE_MISMATCH_ON_OVERRIDE", "VAR_TYPE_MISMATCH_ON_OVERRIDE", "RETURN_TYPE_MISMATCH_ON_INHERITANCE", "PROPERTY_TYPE_MISMATCH_ON_INHERITANCE", "VAR_TYPE_MISMATCH_ON_INHERITANCE", "OVERRIDING_FINAL_MEMBER_BY_DELEGATION", "VAR_OVERRIDDEN_BY_VAL_BY_DELEGATION", "RETURN_TYPE_MISMATCH_BY_DELEGATION", "PROPERTY_TYPE_MISMATCH_BY_DELEGATION", "CONFLICTING_INHERITED_MEMBERS", "CONFLICTING_INHERITED_MEMBERS_WARNING", "ABSTRACT_MEMBER_NOT_IMPLEMENTED", "ABSTRACT_CLASS_MEMBER_NOT_IMPLEMENTED", "ABSTRACT_CLASS_MEMBER_NOT_IMPLEMENTED_WARNING", "MANY_IMPL_MEMBER_NOT_IMPLEMENTED", "MANY_INTERFACES_MEMBER_NOT_IMPLEMENTED", "MANY_INTERFACES_MEMBER_NOT_IMPLEMENTED_WARNING", "AMBIGUOUS_ANONYMOUS_TYPE_INFERRED", "APPROXIMATED_LOCAL_TYPE_WILL_BECOME_NULLABLE", "APPROXIMATED_LOCAL_TYPE_WILL_BECOME_FLEXIBLE", "KCLASS_WITH_NULLABLE_TYPE_PARAMETER_IN_SIGNATURE", "VAR_OVERRIDDEN_BY_VAL", "REDUNDANT_MODIFIER_IN_GETTER", "GETTER_VISIBILITY_DIFFERS_FROM_PROPERTY_VISIBILITY", "SETTER_VISIBILITY_INCONSISTENT_WITH_PROPERTY_VISIBILITY", "PRIVATE_SETTER_FOR_ABSTRACT_PROPERTY", "PRIVATE_SETTER_FOR_OPEN_PROPERTY", "WRONG_GETTER_RETURN_TYPE", "WRONG_SETTER_RETURN_TYPE", "ABSTRACT_PROPERTY_IN_PRIMARY_CONSTRUCTOR_PARAMETERS", "ABSTRACT_PROPERTY_WITH_INITIALIZER", "ABSTRACT_PROPERTY_WITH_GETTER", "ABSTRACT_PROPERTY_WITH_SETTER", "ABSTRACT_DELEGATED_PROPERTY", "ACCESSOR_FOR_DELEGATED_PROPERTY", "DELEGATED_PROPERTY_IN_INTERFACE", "PROPERTY_WITH_NO_TYPE_NO_INITIALIZER", "MUST_BE_INITIALIZED", "MUST_BE_INITIALIZED_OR_BE_ABSTRACT", "EXTENSION_PROPERTY_MUST_HAVE_ACCESSORS_OR_BE_ABSTRACT", "UNNECESSARY_LATEINIT", "EXTENSION_PROPERTY_WITH_BACKING_FIELD", "CONTEXT_RECEIVERS_WITH_BACKING_FIELD", "PROPERTY_INITIALIZER_NO_BACKING_FIELD", "PROPERTY_INITIALIZER_IN_INTERFACE", "PRIVATE_PROPERTY_IN_INTERFACE", "BACKING_FIELD_IN_INTERFACE", "INAPPLICABLE_LATEINIT_MODIFIER", "LATEINIT_INTRINSIC_CALL_ON_NON_LITERAL", "LATEINIT_INTRINSIC_CALL_ON_NON_LATEINIT", "LATEINIT_INTRINSIC_CALL_IN_INLINE_FUNCTION", "LATEINIT_INTRINSIC_CALL_ON_NON_ACCESSIBLE_PROPERTY", "ABSTRACT_PROPERTY_IN_NON_ABSTRACT_CLASS", "VAL_WITH_SETTER", "SETTER_PARAMETER_WITH_DEFAULT_VALUE", "WRONG_SETTER_PARAMETER_TYPE", "ABSTRACT_FUNCTION_IN_NON_ABSTRACT_CLASS", "ABSTRACT_FUNCTION_WITH_BODY", "NON_ABSTRACT_FUNCTION_WITH_NO_BODY", "PRIVATE_FUNCTION_WITH_NO_BODY", "NON_MEMBER_FUNCTION_NO_BODY", "FUNCTION_DECLARATION_WITH_NO_NAME", "ANONYMOUS_FUNCTION_WITH_NAME", "VALUE_PARAMETER_WITH_NO_TYPE_ANNOTATION", "NO_TAIL_CALLS_FOUND", "ANONYMOUS_FUNCTION_PARAMETER_WITH_DEFAULT_VALUE", "USELESS_VARARG_ON_PARAMETER", "MULTIPLE_VARARG_PARAMETERS", "FORBIDDEN_VARARG_PARAMETER_TYPE", "CHANGING_ARGUMENTS_EXECUTION_ORDER_FOR_NAMED_VARARGS", "DEFAULT_VALUE_NOT_ALLOWED_IN_OVERRIDE", "MULTIPLE_DEFAULTS_INHERITED_FROM_SUPERTYPES", "MULTIPLE_DEFAULTS_INHERITED_FROM_SUPERTYPES_WHEN_NO_EXPLICIT_OVERRIDE", "PARAMETER_NAME_CHANGED_ON_OVERRIDE", "DIFFERENT_NAMES_FOR_THE_SAME_PARAMETER_IN_SUPERTYPES", "NAME_FOR_AMBIGUOUS_PARAMETER", "DATA_CLASS_WITHOUT_PARAMETERS", "DATA_CLASS_VARARG_PARAMETER", "DATA_CLASS_NOT_PROPERTY_PARAMETER", "DATA_OBJECT_CUSTOM_EQUALS_OR_HASH_CODE", "CATCH_PARAMETER_WITH_DEFAULT_VALUE", "EXPECTED_DECLARATION_WITH_BODY", "EXPECTED_CLASS_CONSTRUCTOR_DELEGATION_CALL", "EXPECTED_CLASS_CONSTRUCTOR_PROPERTY_PARAMETER", "EXPECTED_ENUM_CONSTRUCTOR", "EXPECTED_ENUM_ENTRY_WITH_BODY", "EXPECTED_PROPERTY_INITIALIZER", "EXPECTED_DELEGATED_PROPERTY", "EXPECTED_LATEINIT_PROPERTY", "SUPERTYPE_INITIALIZED_IN_EXPECTED_CLASS", "EXPECTED_PRIVATE_DECLARATION", "IMPLEMENTATION_BY_DELEGATION_IN_EXPECT_CLASS", "ACTUAL_TYPE_ALIAS_NOT_TO_CLASS", "ACTUAL_TYPE_ALIAS_TO_CLASS_WITH_DECLARATION_SITE_VARIANCE", "ACTUAL_TYPE_ALIAS_WITH_USE_SITE_VARIANCE", "ACTUAL_TYPE_ALIAS_WITH_COMPLEX_SUBSTITUTION", "ACTUAL_FUNCTION_WITH_DEFAULT_ARGUMENTS", "ACTUAL_ANNOTATION_CONFLICTING_DEFAULT_ARGUMENT_VALUE", "EXPECTED_FUNCTION_SOURCE_WITH_DEFAULT_ARGUMENTS_NOT_FOUND", "NO_ACTUAL_FOR_EXPECT", "ACTUAL_WITHOUT_EXPECT", "AMBIGUOUS_ACTUALS", "AMBIGUOUS_EXPECTS", "NO_ACTUAL_CLASS_MEMBER_FOR_EXPECTED_CLASS", "ACTUAL_MISSING", "OPTIONAL_EXPECTATION_NOT_ON_EXPECTED", "OPTIONAL_DECLARATION_OUTSIDE_OF_ANNOTATION_ENTRY", "OPTIONAL_DECLARATION_USAGE_IN_NON_COMMON_SOURCE", "NAME_SHADOWING", "ACCESSOR_PARAMETER_NAME_SHADOWING", "MIXING_NAMED_AND_POSITIONED_ARGUMENTS", "ARGUMENT_PASSED_TWICE", "NAMED_PARAMETER_NOT_FOUND", "NAMED_ARGUMENTS_NOT_ALLOWED", "VARARG_OUTSIDE_PARENTHESES", "SPREAD_OF_NULLABLE", "SPREAD_OF_LAMBDA_OR_CALLABLE_REFERENCE", "MANY_LAMBDA_EXPRESSION_ARGUMENTS", "UNEXPECTED_TRAILING_LAMBDA_ON_A_NEW_LINE", "TOO_MANY_ARGUMENTS", "NO_VALUE_FOR_PARAMETER", "MISSING_RECEIVER", "NO_RECEIVER_ALLOWED", "REDUNDANT_SPREAD_OPERATOR_IN_NAMED_FORM_IN_FUNCTION", "REDUNDANT_SPREAD_OPERATOR_IN_NAMED_FORM_IN_ANNOTATION", "ILLEGAL_SELECTOR", "FUNCTION_EXPECTED", "FUNCTION_CALL_EXPECTED", "NON_TAIL_RECURSIVE_CALL", "TAIL_RECURSION_IN_TRY_IS_NOT_SUPPORTED", "NO_CONSTRUCTOR", "NO_CONSTRUCTOR_WARNING", "CREATING_AN_INSTANCE_OF_ABSTRACT_CLASS", "NOT_A_CLASS", "OVERLOAD_RESOLUTION_AMBIGUITY", "OVERLOAD_RESOLUTION_AMBIGUITY_BECAUSE_OF_STUB_TYPES", "STUB_TYPE_IN_ARGUMENT_CAUSES_AMBIGUITY", "STUB_TYPE_IN_RECEIVER_CAUSES_AMBIGUITY", "BUILDER_INFERENCE_MULTI_LAMBDA_RESTRICTION", "BUILDER_INFERENCE_STUB_RECEIVER", "NONE_APPLICABLE", "CANNOT_COMPLETE_RESOLVE", "UNRESOLVED_REFERENCE_WRONG_RECEIVER", "CALLABLE_REFERENCE_RESOLUTION_AMBIGUITY", "TYPE_PARAMETER_AS_REIFIED", "DEFINITELY_NON_NULLABLE_AS_REIFIED", "REIFIED_TYPE_FORBIDDEN_SUBSTITUTION", "REIFIED_TYPE_UNSAFE_SUBSTITUTION", "CANDIDATE_CHOSEN_USING_OVERLOAD_RESOLUTION_BY_LAMBDA_ANNOTATION", "COMPATIBILITY_WARNING", "RESOLUTION_TO_CLASSIFIER", "RESERVED_SYNTAX_IN_CALLABLE_REFERENCE_LHS", "PARENTHESIZED_COMPANION_LHS_DEPRECATION", "RESOLUTION_TO_PRIVATE_CONSTRUCTOR_OF_SEALED_CLASS", "TYPE_MISMATCH_WARNING_FOR_INCORRECT_CAPTURE_APPROXIMATION", "RECEIVER_TYPE_MISMATCH_WARNING_FOR_INCORRECT_CAPTURE_APPROXIMATION", "CANNOT_INFER_PARAMETER_TYPE", "TYPE_INFERENCE_NO_INFORMATION_FOR_PARAMETER", "NEW_INFERENCE_NO_INFORMATION_FOR_PARAMETER", "INFERRED_INTO_DECLARED_UPPER_BOUNDS", "COULD_BE_INFERRED_ONLY_WITH_UNRESTRICTED_BUILDER_INFERENCE", "TYPE_INFERENCE_CONFLICTING_SUBSTITUTIONS", "TYPE_INFERENCE_CANNOT_CAPTURE_TYPES", "TYPE_INFERENCE_PARAMETER_CONSTRAINT_ERROR", "TYPE_INFERENCE_INCORPORATION_ERROR", "INFERRED_TYPE_VARIABLE_INTO_POSSIBLE_EMPTY_INTERSECTION", "TYPE_INFERENCE_UPPER_BOUND_VIOLATED", "TYPE_INFERENCE_EXPECTED_TYPE_MISMATCH", "TYPE_INFERENCE_CANDIDATE_WITH_SAM_AND_VARARG", "TYPE_INFERENCE_POSTPONED_VARIABLE_IN_RECEIVER_TYPE", "TYPE_INFERENCE_FAILED_ON_SPECIAL_CONSTRUCT", "IMPLICIT_NOTHING_TYPE_ARGUMENT_IN_RETURN_POSITION", "IMPLICIT_NOTHING_TYPE_ARGUMENT_AGAINST_NOT_NOTHING_EXPECTED_TYPE", "EXTENSION_IN_CLASS_REFERENCE_NOT_ALLOWED", "CALLABLE_REFERENCE_LHS_NOT_A_CLASS", "CALLABLE_REFERENCE_TO_ANNOTATION_CONSTRUCTOR", "CLASS_LITERAL_LHS_NOT_A_CLASS", "ARRAY_CLASS_LITERAL_REQUIRES_ARGUMENT", "NULLABLE_TYPE_IN_CLASS_LITERAL_LHS", "EXPRESSION_OF_NULLABLE_TYPE_IN_CLASS_LITERAL_LHS", "ADAPTED_CALLABLE_REFERENCE_AGAINST_REFLECTION_TYPE", "INITIALIZER_REQUIRED_FOR_DESTRUCTURING_DECLARATION", "COMPONENT_FUNCTION_MISSING", "COMPONENT_FUNCTION_ON_NULLABLE", "COMPONENT_FUNCTION_AMBIGUITY", "COMPONENT_FUNCTION_RETURN_TYPE_MISMATCH", "SUPER_IS_NOT_AN_EXPRESSION", "SUPER_CANT_BE_EXTENSION_RECEIVER", "SUPER_NOT_AVAILABLE", "SUPERCLASS_NOT_ACCESSIBLE_FROM_INTERFACE", "AMBIGUOUS_SUPER", "ABSTRACT_SUPER_CALL", "ABSTRACT_SUPER_CALL_WARNING", "NOT_A_SUPERTYPE", "TYPE_ARGUMENTS_REDUNDANT_IN_SUPER_QUALIFIER", "QUALIFIED_SUPERTYPE_EXTENDED_BY_OTHER_SUPERTYPE", "DEPRECATED_IDENTITY_EQUALS", "IMPLICIT_BOXING_IN_IDENTITY_EQUALS", "FORBIDDEN_IDENTITY_EQUALS", "FORBIDDEN_SYNCHRONIZED_BY_VALUE_CLASSES_OR_PRIMITIVES", "DEPRECATED_BINARY_MOD", "FORBIDDEN_BINARY_MOD", "DEPRECATED_BINARY_MOD_AS_REM", "FORBIDDEN_BINARY_MOD_AS_REM", "NO_GET_METHOD", "NO_SET_METHOD", "INC_DEC_SHOULD_NOT_RETURN_UNIT", "ASSIGNMENT_OPERATOR_SHOULD_RETURN_UNIT", "ASSIGN_OPERATOR_AMBIGUITY", "EQUALS_MISSING", "EQUALITY_NOT_APPLICABLE", "EQUALITY_NOT_APPLICABLE_WARNING", "INCOMPATIBLE_ENUM_COMPARISON", "INCOMPATIBLE_ENUM_COMPARISON_ERROR", "HAS_NEXT_MISSING", "HAS_NEXT_FUNCTION_AMBIGUITY", "HAS_NEXT_FUNCTION_NONE_APPLICABLE", "HAS_NEXT_FUNCTION_TYPE_MISMATCH", "NEXT_AMBIGUITY", "NEXT_MISSING", "NEXT_NONE_APPLICABLE", "ITERATOR_MISSING", "ITERATOR_ON_NULLABLE", "ITERATOR_AMBIGUITY", "DELEGATE_SPECIAL_FUNCTION_MISSING", "DELEGATE_SPECIAL_FUNCTION_AMBIGUITY", "DELEGATE_SPECIAL_FUNCTION_NONE_APPLICABLE", "DELEGATE_SPECIAL_FUNCTION_RETURN_TYPE_MISMATCH", "DELEGATE_PD_METHOD_NONE_APPLICABLE", "COMPARE_TO_TYPE_MISMATCH", "YIELD_IS_RESERVED", "UNDERSCORE_IS_RESERVED", "UNDERSCORE_USAGE_WITHOUT_BACKTICKS", "RESOLVED_TO_UNDERSCORE_NAMED_CATCH_PARAMETER", "INVALID_CHARACTERS", "INAPPLICABLE_OPERATOR_MODIFIER", "INAPPLICABLE_INFIX_MODIFIER", "OPERATOR_MODIFIER_REQUIRED", "INFIX_MODIFIER_REQUIRED", "PROPERTY_AS_OPERATOR", "INAPPLICABLE_MODIFIER", "DSL_SCOPE_VIOLATION", "DSL_SCOPE_VIOLATION_WARNING", "NULLABLE_EXTENSION_OPERATOR_WITH_SAFE_CALL_RECEIVER", "LABEL_NAME_CLASH", "LABEL_RESOLVE_WILL_CHANGE", "AMBIGUOUS_LABEL", "BREAK_OR_CONTINUE_OUTSIDE_A_LOOP", "BREAK_OR_CONTINUE_IN_WHEN", "BREAK_OR_CONTINUE_JUMPS_ACROSS_FUNCTION_BOUNDARY", "NOT_A_LOOP_LABEL", "NOT_A_FUNCTION_LABEL", "NOT_A_FUNCTION_LABEL_WARNING", "REDUNDANT_LABEL_WARNING", "UNREACHABLE_CODE", "VARIABLE_WITH_NO_TYPE_NO_INITIALIZER", "UNINITIALIZED_VARIABLE", "UNINITIALIZED_PARAMETER", "UNINITIALIZED_PARAMETER_WARNING", "UNINITIALIZED_ENUM_ENTRY", "UNINITIALIZED_ENUM_COMPANION", "UNINITIALIZED_ENUM_COMPANION_WARNING", "UNUSED_VARIABLE", "UNUSED_PARAMETER", "UNUSED_ANONYMOUS_PARAMETER", "UNUSED_DESTRUCTURED_PARAMETER_ENTRY", "UNUSED_TYPEALIAS_PARAMETER", "ASSIGNED_BUT_NEVER_ACCESSED_VARIABLE", "VARIABLE_WITH_REDUNDANT_INITIALIZER", "UNUSED_VALUE", "UNUSED_CHANGED_VALUE", "UNUSED_EXPRESSION", "UNUSED_LAMBDA_EXPRESSION", "VAL_REASSIGNMENT", "CAPTURED_VAL_INITIALIZATION", "CAPTURED_MEMBER_VAL_INITIALIZATION", "SETTER_PROJECTED_OUT", "INITIALIZATION_BEFORE_DECLARATION", "VARIABLE_EXPECTED", "SENSELESS_COMPARISON", "SENSELESS_NULL_IN_WHEN", "INVALID_IF_AS_EXPRESSION", "INVALID_IF_AS_EXPRESSION_WARNING", "UNSAFE_CALL", "UNSAFE_IMPLICIT_INVOKE_CALL", "UNSAFE_INFIX_CALL", "UNSAFE_OPERATOR_CALL", "UNNECESSARY_SAFE_CALL", "SAFE_CALL_WILL_CHANGE_NULLABILITY", "UNEXPECTED_SAFE_CALL", "UNNECESSARY_NOT_NULL_ASSERTION", "NOT_NULL_ASSERTION_ON_LAMBDA_EXPRESSION", "NOT_NULL_ASSERTION_ON_CALLABLE_REFERENCE", "USELESS_ELVIS", "USELESS_ELVIS_RIGHT_IS_NULL", "DIVISION_BY_ZERO", "INTEGER_OVERFLOW", "WRONG_LONG_SUFFIX", "INT_LITERAL_OUT_OF_RANGE", "FLOAT_LITERAL_OUT_OF_RANGE", "FLOAT_LITERAL_CONFORMS_INFINITY", "FLOAT_LITERAL_CONFORMS_ZERO", "CONSTANT_EXPECTED_TYPE_MISMATCH", "INCORRECT_CHARACTER_LITERAL", "EMPTY_CHARACTER_LITERAL", "ILLEGAL_UNDERSCORE", "TOO_MANY_CHARACTERS_IN_CHARACTER_LITERAL", "ILLEGAL_ESCAPE", "NULL_FOR_NONNULL_TYPE", "NULL_FOR_NONNULL_TYPE_WARNING", "ILLEGAL_ESCAPE_SEQUENCE", "UNSIGNED_LITERAL_WITHOUT_DECLARATIONS_ON_CLASSPATH", "SIGNED_CONSTANT_CONVERTED_TO_UNSIGNED", "INTEGER_OPERATOR_RESOLVE_WILL_CHANGE", "NON_TRIVIAL_BOOLEAN_CONSTANT", "CANNOT_CHECK_FOR_ERASED", "UNCHECKED_CAST", "USELESS_CAST", "CAST_NEVER_SUCCEEDS", "DYNAMIC_NOT_ALLOWED", "IS_ENUM_ENTRY", "ENUM_ENTRY_AS_TYPE", "IMPLICIT_CAST_TO_ANY", "SMARTCAST_IMPOSSIBLE", "DEPRECATED_SMARTCAST", "ALWAYS_NULL", "USELESS_NULLABLE_CHECK", "USELESS_IS_CHECK", "LOCAL_EXTENSION_PROPERTY", "LOCAL_VARIABLE_WITH_GETTER", "LOCAL_VARIABLE_WITH_SETTER", "LOCAL_VARIABLE_WITH_TYPE_PARAMETERS_WARNING", "LOCAL_VARIABLE_WITH_TYPE_PARAMETERS", "INVISIBLE_SETTER", "VAL_OR_VAR_ON_LOOP_PARAMETER", "VAL_OR_VAR_ON_FUN_PARAMETER", "VAL_OR_VAR_ON_CATCH_PARAMETER", "VAL_OR_VAR_ON_SECONDARY_CONSTRUCTOR_PARAMETER", "EXPECTED_CONDITION", "ELSE_MISPLACED_IN_WHEN", "REDUNDANT_ELSE_IN_WHEN", "NO_ELSE_IN_WHEN", "NO_ELSE_IN_WHEN_WARNING", "NON_EXHAUSTIVE_WHEN", "NON_EXHAUSTIVE_WHEN_STATEMENT", "NON_EXHAUSTIVE_WHEN_ON_SEALED_CLASS", "EXPECT_TYPE_IN_WHEN_WITHOUT_ELSE", "COMMA_IN_WHEN_CONDITION_WITHOUT_ARGUMENT", "DUPLICATE_LABEL_IN_WHEN", "ILLEGAL_DECLARATION_IN_WHEN_SUBJECT", "TYPE_MISMATCH", "TYPE_MISMATCH_WARNING", "TYPE_MISMATCH_DUE_TO_EQUALS_LAMBDA_IN_FUN", "TYPE_MISMATCH_DUE_TO_TYPE_PROJECTIONS", "MEMBER_PROJECTED_OUT", "RETURN_TYPE_MISMATCH", "EXPECTED_TYPE_MISMATCH", "ASSIGNMENT_TYPE_MISMATCH", "TYPE_MISMATCH_IN_FOR_LOOP", "RESULT_TYPE_MISMATCH", "TYPE_MISMATCH_IN_RANGE", "EXPECTED_PARAMETER_TYPE_MISMATCH", "EXPECTED_PARAMETER_TYPE_MISMATCH_WARNING", "EXPECTED_PARAMETERS_NUMBER_MISMATCH", "INCOMPATIBLE_TYPES", "IMPLICIT_NOTHING_RETURN_TYPE", "IMPLICIT_NOTHING_PROPERTY_TYPE", "ABBREVIATED_NOTHING_RETURN_TYPE", "ABBREVIATED_NOTHING_PROPERTY_TYPE", "IMPLICIT_INTERSECTION_TYPE", "DYNAMIC_RECEIVER_NOT_ALLOWED", "EXPRESSION_EXPECTED", "ASSIGNMENT_IN_EXPRESSION_CONTEXT", "DECLARATION_IN_ILLEGAL_CONTEXT", "EXPRESSION_EXPECTED_PACKAGE_FOUND", "RETURN_NOT_ALLOWED", "RETURN_IN_FUNCTION_WITH_EXPRESSION_BODY", "NO_RETURN_IN_FUNCTION_WITH_BLOCK_BODY", "NO_RETURN_IN_FUNCTION_WITH_BLOCK_BODY_MIGRATION", "ANONYMOUS_INITIALIZER_IN_INTERFACE", "NO_THIS", "NO_COMPANION_OBJECT", "TYPE_PARAMETER_IS_NOT_AN_EXPRESSION", "TYPE_PARAMETER_ON_LHS_OF_DOT", "NESTED_CLASS_ACCESSED_VIA_INSTANCE_REFERENCE", "NESTED_CLASS_SHOULD_BE_QUALIFIED", "INACCESSIBLE_OUTER_CLASS_EXPRESSION", "NESTED_CLASS_NOT_ALLOWED", "NESTED_CLASS_DEPRECATED", "NON_PUBLIC_CALL_FROM_PUBLIC_INLINE", "PRIVATE_CLASS_MEMBER_FROM_INLINE", "NON_LOCAL_RETURN_NOT_ALLOWED", "NOT_YET_SUPPORTED_IN_INLINE", "NOTHING_TO_INLINE", "USAGE_IS_NOT_INLINABLE", "USAGE_IS_NOT_INLINABLE_WARNING", "NULLABLE_INLINE_PARAMETER", "RECURSION_IN_INLINE", "DECLARATION_CANT_BE_INLINED", "DECLARATION_CANT_BE_INLINED_WARNING", "OVERRIDE_BY_INLINE", "REIFIED_TYPE_PARAMETER_IN_OVERRIDE", "INLINE_CALL_CYCLE", "NON_LOCAL_RETURN_IN_DISABLED_INLINE", "INLINE_PROPERTY_WITH_BACKING_FIELD", "NON_INTERNAL_PUBLISHED_API", "INVALID_DEFAULT_FUNCTIONAL_PARAMETER_FOR_INLINE", "NOT_SUPPORTED_INLINE_PARAMETER_IN_INLINE_PARAMETER_DEFAULT_VALUE", "PRIVATE_INLINE_FUNCTIONS_RETURNING_ANONYMOUS_OBJECTS", "NON_LOCAL_SUSPENSION_POINT", "ILLEGAL_SUSPEND_FUNCTION_CALL", "ILLEGAL_SUSPEND_PROPERTY_ACCESS", "ILLEGAL_RESTRICTED_SUSPENDING_FUNCTION_CALL", "NON_MODIFIER_FORM_FOR_BUILT_IN_SUSPEND", "RETURN_FOR_BUILT_IN_SUSPEND", "MODIFIER_FORM_FOR_NON_BUILT_IN_SUSPEND", "PLUGIN_ERROR", "PLUGIN_WARNING", "PLUGIN_INFO", "ERROR_IN_CONTRACT_DESCRIPTION", "CONTRACT_NOT_ALLOWED", "NO_CONTEXT_RECEIVER", "MULTIPLE_ARGUMENTS_APPLICABLE_FOR_CONTEXT_RECEIVER", "AMBIGUOUS_CALL_WITH_IMPLICIT_CONTEXT_RECEIVER", "UNSUPPORTED_CONTEXTUAL_DECLARATION_CALL", "SUBTYPING_BETWEEN_CONTEXT_RECEIVERS")
```
