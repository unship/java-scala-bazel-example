rules_scala_version="d916599d38de29085e5ca9eae167716c4f150a02" # update this as needed

http_archive(
             name = "io_bazel_rules_scala",
             url = "https://github.com/bazelbuild/rules_scala/archive/%s.zip"%rules_scala_version,
             type = "zip",
             strip_prefix= "rules_scala-%s" % rules_scala_version
)

load("@io_bazel_rules_scala//scala:scala.bzl", "scala_repositories")
scala_repositories()

load("@io_bazel_rules_scala//specs2:specs2_junit.bzl","specs2_junit_repositories")
specs2_junit_repositories()

maven_jar(name = "org_hamcrest_hamcrest_core_1_3", artifact = "org.hamcrest:hamcrest-core:jar:1.3")
maven_jar(name = "junit_junit_4_12", artifact = "junit:junit:jar:4.12")


maven_jar(name = "org_scala_lang_scala_library_2_11_11", artifact = "org.scala-lang:scala-library:jar:2.11.11")
maven_jar(name = "org_scala_lang_modules_scala_parser_combinators_2_11_1_0_4", artifact = "org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4")
maven_jar(name = "org_scala_lang_scala_reflect_2_11_11", artifact = "org.scala-lang:scala-reflect:jar:2.11.11")
maven_jar(name = "org_scala_lang_modules_scala_xml_2_11_1_0_5", artifact = "org.scala-lang.modules:scala-xml_2.11:jar:1.0.5")
maven_jar(name = "org_scalactic_scalactic_2_11_3_2_0_SNAP7", artifact = "org.scalactic:scalactic_2.11:jar:3.2.0-SNAP7")
maven_jar(name = "org_scalatest_scalatest_2_11_3_2_0_SNAP7", artifact = "org.scalatest:scalatest_2.11:jar:3.2.0-SNAP7")


maven_jar(name = "org_ow2_asm_asm_4_1", artifact = "org.ow2.asm:asm:jar:4.1")
maven_jar(name = "org_ow2_asm_asm_analysis_4_1", artifact = "org.ow2.asm:asm-analysis:jar:4.1")
maven_jar(name = "org_ow2_asm_asm_tree_4_1", artifact = "org.ow2.asm:asm-tree:jar:4.1")
maven_jar(name = "org_ow2_asm_asm_util_4_1", artifact = "org.ow2.asm:asm-util:jar:4.1")
maven_jar(name = "org_specs2_classycle_1_4_3", artifact = "org.specs2:classycle:jar:1.4.3")

# duplicate maven_jar(name = "org_hamcrest_hamcrest_core_1_3", artifact = "org.hamcrest:hamcrest-core:jar:1.3")
maven_jar(name = "junit_junit_4_11", artifact = "junit:junit:jar:4.11")
maven_jar(name = "org_mockito_mockito_core_1_9_5", artifact = "org.mockito:mockito-core:jar:1.9.5")
maven_jar(name = "org_objenesis_objenesis_1_0", artifact = "org.objenesis:objenesis:jar:1.0")
maven_jar(name = "org_parboiled_parboiled_core_1_1_4", artifact = "org.parboiled:parboiled-core:jar:1.1.4")
maven_jar(name = "org_parboiled_parboiled_java_1_1_4", artifact = "org.parboiled:parboiled-java:jar:1.1.4")
maven_jar(name = "org_pegdown_pegdown_1_2_1", artifact = "org.pegdown:pegdown:jar:1.2.1")
maven_jar(name = "org_scalamacros_quasiquotes_2_10_2_0_1", artifact = "org.scalamacros:quasiquotes_2.10:jar:2.0.1")
maven_jar(name = "org_scala_lang_scala_compiler_2_10_5", artifact = "org.scala-lang:scala-compiler:jar:2.10.5")
maven_jar(name = "org_scala_lang_scala_library_2_10_5", artifact = "org.scala-lang:scala-library:jar:2.10.5")
maven_jar(name = "org_scala_lang_scala_reflect_2_10_5", artifact = "org.scala-lang:scala-reflect:jar:2.10.5")
maven_jar(name = "org_scalacheck_scalacheck_2_10_1_12_2", artifact = "org.scalacheck:scalacheck_2.10:jar:1.12.2")
maven_jar(name = "org_scalaz_scalaz_concurrent_2_10_7_1_1", artifact = "org.scalaz:scalaz-concurrent_2.10:jar:7.1.1")
maven_jar(name = "org_scalaz_scalaz_core_2_10_7_1_1", artifact = "org.scalaz:scalaz-core_2.10:jar:7.1.1")
maven_jar(name = "org_scalaz_scalaz_effect_2_10_7_1_1", artifact = "org.scalaz:scalaz-effect_2.10:jar:7.1.1")
maven_jar(name = "org_scalaz_stream_scalaz_stream_2_10_0_7a", artifact = "org.scalaz.stream:scalaz-stream_2.12:0.8.6")
maven_jar(name = "org_specs2_specs2_2_10_3_3_1", artifact = "org.specs2:specs2_2.10:jar:3.3.1")
maven_jar(name = "org_ccil_cowan_tagsoup_tagsoup_1_2", artifact = "org.ccil.cowan.tagsoup:tagsoup:jar:1.2")